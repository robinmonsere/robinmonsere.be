<script>
import logo from "$lib/images/R logo.png";
</script>

<div id="top">
    <a href="/">
        <img src={logo} alt="R Logo" />
    </a>
    <nav>
        <a href="/#about">About</a>
        <a href="/#skills">Skills</a>
        <a href="/#projects">Projects</a>
    </nav>
</div>

<style>

    #top {
        position: sticky;
        top: 10px ;
        margin-top: 2rem;
        margin-bottom: 1rem;
        display: flex;
        flex-direction: row;
        justify-content: space-between;
    }

    nav {
        width: 12rem;
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        font-weight: bold;
    }

    nav a:hover {
        color: var(--color-theme-1);
    }

    #top img {
        width: 2.5rem;
    }
</style>