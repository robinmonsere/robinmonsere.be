<script>
    import starbase from '$lib/images/blog/starbase.jpg'
    let date;
    let title;
    let text;
</script>

<div id="blogPost">
    <img src="{starbase}" alt="">
    <div id="information">
        <h2>{title}</h2>
        <p>{text}</p>
        <p id="date">{date}</p>
    </div>
</div>

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
        border-radius: 0.4rem 0.4rem 0 0;
    }

    h2 {
        color: var(--color-theme-1);
        font-weight: bold;
        font-size: 1.5rem;
    }

    #date {
        color: var(--color-text-2);
    }
</style>