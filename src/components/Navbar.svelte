<script>

    let fixed = false
    let isOpen = false
    let y = window.scrollY

    $: {
        fixed = y > 72 ? true : false
    }

    const handleClick = () => isOpen = !isOpen


</script>

<svelte:window bind:scrollY={y} />

<div class={fixed ? 'fixed-navbar': ''}>
    <nav>
        <img src="/img/Logo.svg" alt="logo site" />
        <div>
            <img src="/img/Menu.svg" alt="Menu site" class="menu-burger" on:click={handleClick} />
            <ul class={isOpen ? 'show-menu' : ''}>
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

        transition: .3s all ease;
    }

    ul {
        display: none;
        font-weight: 500;
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
            gap: 2rem;
            display:flex;
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

    nav > div {
        position: relative;
    }

    @media(max-width: 1024px) {
        .show-menu {
        display: flex;
        position: absolute;
        flex-direction: column;
        top: 30px;
        right: 0;
        background-color: var(--primary);
        box-sizing: border-box;
    }

    .show-menu li {
        padding: .5rem 2rem;
    }
    }

</style>