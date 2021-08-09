<section id="projects">
    <h3>Projects</h3>
    <div class="projects-grid" >
        <slot></slot>
        <div class="btn-more">
            <a href="." class="btn btn-secondary">More Projects</a>
        </div>
    </div>
</section>

<style>
    section {

        width: 90%;
        max-width: 1190px;
        margin: 0 auto;
        color: var(--gray900);
        padding: 2.5em 0;
        width: 90%;
    }

    h3 {
        margin-bottom: 2rem;
        text-align: center;
    }

    .projects-grid {
        display: grid;
        gap: 4rem;
    }

    .btn-more a {
        box-shadow: 0px 0px 15px -5px rgba(0,0,0,0.5);
    }

    @media(min-width: 767px) {
        section {
            font-size: 13px;
        }

        .projects-grid {
            gap: 8rem;
        }

        h3 {
            margin-bottom: 4rem;
        }
    }

    @media(min-width: 1024px) {

        section {
            font-size: 16px;
        }

        .projects-grid {
            gap: 9.25rem;
        }

        .btn-more {
            display: flex;
            justify-content: center;
        }
    }
</style>