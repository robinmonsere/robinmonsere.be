<script>
    import logo from '$lib/images/R logo.png';
    import {page} from "$app/stores";
</script>

<div>
    <button>
        <p>View my blog</p>
    </button>
    <nav>
        <ul>
            <li><a href="/#about">About</a></li>
            <li><a href="/#skills">Skills</a></li>
            <li><a href="/#projects">Projects</a></li>
        </ul>
    </nav>
</div>
    <!--
    <div class="corner">
        <a href="https://robinmonsere.be">
            <img src={logo} alt="R Logo" />
        </a>
    </div>
    -->


<style>

    div {
        margin-top: 1rem;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
    }

    button {
        margin-bottom: 2rem;
        color: white;
        background: none;
        width: 10rem;
        height: 2rem;
        border: 1px white solid;
        border-radius: 0.2rem;

    }

    button:hover {
        background: white;
        color: black;
    }

    .corner img {
        color: white;
        width: 5rem;
        height: 5rem;
        object-fit: contain;
    }

    ul {
        list-style: none;
    }

    li {
        margin-bottom: 1rem;
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