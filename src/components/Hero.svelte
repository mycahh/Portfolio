<section>
    <figure>
        <img src="img/Hero.svg" alt="hero" />
    </figure>
    <div class="hero-content">
        <h2>Web Developer</h2>
        <p>Welcome, I’m Mikael Fernandez, a developer who likes to try new technologies and experiment.</p>
        <div class="buttons">
            <a href="https://github.com" class="btn btn-primary" >
                <img src="/img/github.svg" alt="github icon"/>
                <span>Github</span>
            </a>
            <a href="https://linkedin.com" class="btn btn-primary" >
                <img src="/img/linkedin.svg" alt="linkedin icon"/>
                <span>Linkedin</span>
            </a>
        </div>
    </div>
</section>

<style>
    section {

        font-size: 12px;

        box-sizing: border-box;
        max-width: 90%;

        text-align: center;

        margin: 0 auto;
        padding: 3rem 0;

        display: flex;
        flex-direction: column;

    }

    h2 {
        margin-top: 1.5rem;
    }

    p {
        margin: .8rem 0 2rem 0;
        line-height: 1.5rem;
    }

    a > img {
        height: 1rem;
    }

    img {
        width: 100%;
    }


    a {
        gap: 0.375rem;
    }


    .buttons {
        display: flex;
        justify-content: center;
        gap: 1.4rem;
    }

    @media(min-width: 768px) {
        section {
            flex-direction: row-reverse;
            padding-top: 4rem;
            padding-bottom: 6rem;
            text-align: left;

        }

        section > figure {
            width: 40%;
        }

        section > div {
            width: 60%;
        }

        .btn {
            padding: 10px !important;
        }

        .buttons {
            justify-content: flex-start;
        }
    }

    @media(min-width: 1200px) {
        section {
            max-width: 82%;
            min-height: calc(90vh - 72px);
            box-sizing: border-box;
        }

        .hero-content {
            width: 540px;
        }

        p {
            font-size: 18px;
        }
    }
</style>