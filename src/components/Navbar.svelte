<nav>
    <img src="/img/Logo.svg" alt="logo site" />
    <div>
        <img src="/img/Menu.svg" alt="Menu site" class="menu-burger"/>
        <ul>
            <li>Projects</li>
            <li>Home</li>
            <li>About me</li>
            <li>Contact</li>
        </ul>
    </div>
</nav>

<style>
    nav {
        display: flex;
        justify-content: space-between;
        align-items: center;

        padding: 0 1rem;
        margin: 0 auto;

        max-width: 1200px;
        width: 90%;
        height: var(--height-nav);
    }

    ul {
        display: none;
        font-weight: 500;
        gap: 2rem;
    }

    li {
        cursor: pointer;
    }

    .menu-burger {
        display: block;
        height: 22px;
    }

    @media(min-width: 64rem) {
        .menu-burger {
            display: none;
        }

        ul {
            display: flex;
        }
    }
</style>