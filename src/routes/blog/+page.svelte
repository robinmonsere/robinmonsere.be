<script>
    import logo from '$lib/images/R logo.png'
    import BlogPost from "./BlogPost.svelte";

</script>


<div>
    <h1>Robin Monseré's <span>blog</span></h1>
</div>
<section id="blogPosts">
    <BlogPost></BlogPost>
    <BlogPost></BlogPost>
    <BlogPost></BlogPost>
    <BlogPost></BlogPost>
    <BlogPost></BlogPost>
    <BlogPost></BlogPost>
    <BlogPost></BlogPost>
    <BlogPost></BlogPost>
    <BlogPost></BlogPost>
    <BlogPost></BlogPost>
</section>


<style>
    #blogPosts{
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        justify-content: space-between;
        row-gap: 2rem;
    }

    h1 {
        font-weight: bold;
        font-size: 5rem;
        margin-bottom: 2rem;
        margin-top: 4rem;
    }

    h1 span {
        color: var(--color-theme-1);
    }
</style>