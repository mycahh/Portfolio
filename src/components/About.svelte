<section>
    <article>
        <div>
            <h3>About me</h3>
            <p>Greetings, I am a developer focused on web development, although I am also dedicated to other areas of my interest, I like to try different technologies and take on challenges in projects.
            <br>
            <br>
            As a Frontend developer, I have experience in HTML-CSS-JS and particularly in React, from the creation of landing pages to more complex applications. On the other hand and to a lesser extent I am familiar with the creation of API Rest, and the use of different frameworks to create a backend and database management.</p>
        </div>
        <figure>
            <img src="/img/about.svg" alt="about" />
        </figure>
    </article>
</section>

<style>
    section {
        padding: 2.5em 0;
        color: var(--gray600);

        background-color: var(--primary);
    }

    article {
        margin: 0 auto;
        width: 90%;

        text-align: center;
    }

    figure {
        padding-top: 2rem;
    }

    img {
        width: 80%;
    }

    @media(min-width: 767px) {

        img {
            width: 200px;
            margin: auto;
        }

        figure {
            display: none;
        }
    }

    @media(min-width: 1024px) {

        article {
            display: flex;
            max-width: 82%;
        }

        div {
            text-align: left;
        }

        article > * {
            width: 50%;
        }

        figure {
            display: block;
        }

        figure {
            margin: auto auto;
        }

        figure img {
            width: 336px;
        }
    }
</style>
