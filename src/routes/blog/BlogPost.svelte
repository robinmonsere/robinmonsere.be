<script>
    export let date;
    export let title;
    export let text;
    export let img;
    export let url;
</script>

<a id="blogPost" href="/blog/{url}" >
    <img src="{img}" alt="">
    <div id="information">
        <h2>{title}</h2>
        <p>{text}</p>
        <p id="date">{date}</p>
    </div>
</a>

<style>

    #blogPost {
        border-radius: 0.4rem;
        border: 2px white solid;
        width: 48%;
        background: var(--color-bg-1);
        transition: 0.5s;
    }

    #blogPost:hover {
        scale: 110%;
        cursor: pointer;
    }

    #information {
        padding: 1rem;
    }

    img {
        width: 100%;
        height: 15rem;
        border-radius: 0.4rem 0.4rem 0 0;
        object-fit: cover;
    }

    h2 {
        color: var(--color-theme-1);
        font-weight: bold;
        font-size: 1.5rem;
        padding-bottom: 0.4rem;
    }

    #date {
        padding-top: 0.5rem;
        color: var(--color-text-2);
    }
</style>