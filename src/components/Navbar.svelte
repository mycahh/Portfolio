<script>

    let fixed = false
    let handleMove = () => {}

    function DOMContentLoaded() {
        const Nav = document.querySelector('#navbar-container')

        handleMove = () => {
        if(window.scrollY > 72) {
            Nav.classList.add('fixed-navbar')
            isSticky = true

        } else {
            Nav.classList.remove('fixed-navbar')
            isSticky = false
            }
        }
    }

    window.addEventListener('DOMContentLoaded', DOMContentLoaded)

</script>

<svelte:window on:mousemove={handleMove}/>


<div class={fixed ? 'fixed-navbar': ''} id="navbar-container">
    <nav >
        <img src="/img/Logo.svg" alt="logo site" />
        <div>
            <img src="/img/Menu.svg" alt="Menu site" class="menu-burger"/>
            <ul>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </div>
    </nav>
</div>

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
        z-index: 10;
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

    nav::before {
        display: block;
        position: absolute;
        height: 72px;
        z-index: 0;
        top: 0;
    }

    .fixed-navbar {
        position: fixed;
        width: 100vw;
        background-color: var(--primary);
        border-bottom: 1px solid (--gray600);
    }

    .fixed-navbar nav {
        height: 55px;
    }
</style>