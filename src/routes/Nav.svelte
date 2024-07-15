<script>
    import { page } from '$app/stores';
    import { scrollTo } from 'svelte-scrolling'

    const handleScroll = () => {
        const skillsSection = document.getElementById('skills').offsetTop;
        const projectsSection = document.getElementById('projects').offsetTop;



        const navAbout = document.getElementById('nav-about');
        const navSKills = document.getElementById('nav-skills');
        const navProject = document.getElementById('nav-projects');

        const scrollPosition = window.scrollY;

        if (scrollPosition < skillsSection - 100) {
            navAbout.ariaCurrent = true;
            navSKills.ariaCurrent = false;
            navProject.ariaCurrent = false;
        } else if (scrollPosition < projectsSection - 100) {
            navAbout.ariaCurrent = false;
            navSKills.ariaCurrent = true;
            navProject.ariaCurrent = false;
        } else {
            navAbout.ariaCurrent = false;
            navSKills.ariaCurrent = false;
            navProject.ariaCurrent = true;
        }
    };

</script>

<svelte:document on:scroll={handleScroll} />


<div>
    <div class="button diagonal-tl-br-out">
        <a href="https://github.com/robinmonsere">Take a look at my Github</a>
    </div>
    <nav>
        <a use:scrollTo={{ ref:'about', duration: 1000}} id="nav-about" aria-current={$page.url.hash === '#about' || $page.url.hash === ''} href="/#about"><span class="nav_indicator"></span><span>About</span></a>
        <a use:scrollTo={{ ref: 'skills' , duration: 1000}} id="nav-skills" aria-current={$page.url.hash === '#skills'} href="/#skills"><span class="nav_indicator"></span><span>Skills</span></a>
        <a use:scrollTo={{ ref: 'projects', duration: 1000 }} id="nav-projects" aria-current={$page.url.hash === '#projects'} href="/#projects"><span class="nav_indicator"></span><span>Projects</span></a>
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

    nav {
        display: flex;
        flex-direction: column;
        gap: 0.8rem;
    }

    nav a {
        color: var(--color-text-2);
        font-weight: 700;
        font-size: 0.8rem;
        text-transform: uppercase;
        letter-spacing: 0.1em;
        transition: color 0.2s linear;
        display: flex;
        flex-direction: row;
        align-items: center;
    }

    .nav_indicator {
        margin-right: 0.3rem;
        display: block;
        width: 2rem;
        height: 1px;
        box-sizing: border-box;
        border: 1px solid var(--color-text-2);
        transition-duration: .2s;
    }

    nav a[aria-current=true] span {
        color: var(--color-theme-1);
    }

    nav a[aria-current=true] .nav_indicator {
        width: 4rem;
        color: var(--color-theme-1);
        border: 1px solid var(--color-theme-1);
    }
    
    nav a:hover {
        color: var(--color-theme-1);
    }

    nav a:hover .nav_indicator {
        width: 4rem;
        color: var(--color-theme-1);
        border: 1px solid var(--color-theme-1);
    }

    @media screen and (max-width: 800px) {
        nav {
            display: none;
        }
    }
</style>