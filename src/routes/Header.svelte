<script>
    import logo from '$lib/images/R logo.png';
    import {page} from "$app/stores";
</script>


<header>
    <div class="corner">
        <a href="https://robinmonsere.be">
            <img src={logo} alt="R Logo" />
        </a>
    </div>
    <nav>
        <ul>

            <li><a href="/">Home</a></li>
            <li><a href="/">About</a></li>
            <li><a href="/">Projects</a></li>
            <li><a href="/">Contact</a></li>
            <li aria-current={$page.url.pathname === '/blog' ? 'page' : undefined}><a href="/blog">blog</a></li>
        </ul>
    </nav>

</header>

<style>
    header {
        display: flex;
        justify-content: space-between;
        margin: 2rem;
    }

    .corner img {
        color: white;
        width: 5rem;
        height: 5rem;
        object-fit: contain;
    }

    ul {
        position: relative;
        padding: 0;
        margin: 0;
        height: 3em;
        display: flex;
        justify-content: center;
        align-items: center;
        list-style: none;

        background-size: contain;
    }

    li {
        position: relative;
        height: 100%;
    }

    li[aria-current='page']::before {
        --size: 6px;
        content: '';
        width: 0;
        height: 0;
        position: absolute;
        top: 0;
        left: calc(50% - var(--size));
        border: var(--size) solid transparent;
        border-top: var(--size) solid var(--color-theme-1);
    }

    nav a {
        display: flex;
        height: 100%;
        align-items: center;
        padding: 0 0.5rem;
        color: var(--color-text);
        font-weight: 700;
        font-size: 0.8rem;
        text-transform: uppercase;
        letter-spacing: 0.1em;
        text-decoration: none;
        transition: color 0.2s linear;
    }

    a:hover {
        color: var(--color-theme-1);
    }
</style>