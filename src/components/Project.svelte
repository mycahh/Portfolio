<script>
    export let reverse = false
</script>

<article class={reverse ? 'reverse': ''}>
    <div>
        <h5>Weather App</h5>
        <p>A weather application that allows you to view the current weather and get a forecast for the next few days.</p>
        <div class="projects-buttons">
            <a href="." class="btn btn-primary">Demo</a>
            <a href="." class="btn btn-secondary">Source</a>
        </div>
    </div>
    <figure class="img-project">
        <img src="/img/project1.png" alt="site-logo" />
    </figure>
</article>

<style>
    figure {
        margin: 0;
    }

    figure, img {
        width: 100%;
    }

    .projects-buttons {
        display: flex;
        gap: 18px;
        justify-content: center;
    }

    p {
        margin-bottom: 2rem;
    }

    .projects-buttons a {
        padding: 10px 20px;
    }

    article {
        display: flex;
        flex-direction: column;
        gap: 1.5rem;
    }

    article > figure {
        order: 1;
    }

    article > div {
        order: 2;
    }

    @media(min-width: 768px) {

        article {
            flex-direction: row;
        }

        article > * {
            width: 50%;
        }

        article > figure {
            order: 2;
        }

        article > div {
            order: 1;
        }

        .reverse > figure {
            order: 1;
        }

        .reverse > div {
            order: 2;
        }

        .projects-buttons {
            justify-content: flex-start;
        }
    }

    @media(min-width: 1024px) {
        article > div {
            max-width: 540px;
        }

        figure {
            max-width: 540px;
            margin-left: auto;
        }

        .reverse figure {
            margin-left: 0;
            margin-right: auto;
        }

        h5 {
            font-weight: 600;
        }

        p {
            line-height: 26px;
        }
    }
</style>