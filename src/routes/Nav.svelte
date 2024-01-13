<script>
    import logo from '$lib/images/R logo.png';
    import {page} from "$app/stores";
</script>

<div>
    <div class="button diagonal-tl-br-out">
        <a href="">View my blog</a>
    </div>
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
    .button {
        margin-bottom: 2rem;
        color: white;
        background: none;
        width: 10rem;
        height: 2.5rem;
        border: 2px white solid;
        border-radius: 0.4rem;
        text-align: center;
        overflow: hidden;
        position: relative;
        transition: 1s ease;
        z-index: 1;
    }
    .button:hover {
        color: var(--color-bg-0);
        border: 2px var(--color-bg-0) solid;
    }

    .button:before, .button:after {
        transition: 0.5s ease;
        content: '';
        position: absolute;
        z-index: -1;
    }

    .button a {
        text-align: center;
        padding-top: 0.7rem;
    }

    .diagonal-tl-br-out {
        background: var(--color-theme-1);
    }
    .diagonal-tl-br-out:before, .diagonal-tl-br-out:after {
        background: var(--color-bg-0);
        top: 0;
        bottom: 0;
        transform: skewX(-45deg);
        width: 175%;
    }
    .diagonal-tl-br-out:before {
        left: -120%;
    }
    .diagonal-tl-br-out:after {
        right: -120%;
    }
    .diagonal-tl-br-out:hover:before, .diagonal-tl-br-out:hover:after {
        width: 105%;
    }


    div {
        margin-top: 1rem;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
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
        transition: color 0.2s linear;
    }

    nav a:hover {
        color: var(--color-theme-1);
    }
</style>