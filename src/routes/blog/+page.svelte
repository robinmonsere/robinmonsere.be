<script>
    import logo from '$lib/images/R logo.png'
    import BlogPost from "./BlogPost.svelte";
    import starbase from './images/starbase.jpg'
    import workshop from './images/workshop1.jpg'
    import lieven from './images/LievenAI.png'
    import usa from './images/usa.jpg';
    import {goto} from "$app/navigation";

    function handleClick(){
        console.log("test")
    }
</script>


<div>
    <h1>Robin Monseré's <span>blog</span></h1>
</div>
<section id="blogPosts">
    <BlogPost url="usa" title="International study in the USA" img="{usa}" text="" date="15/08/2023 - 6/01/2024"></BlogPost>
    <BlogPost url="ift-2" title="Starship IFT-2" img="{starbase}" text="Witnessing the second test flight of the largest rocket ever made" date="18/11/2023"></BlogPost>
    <BlogPost url="workshop-vti" title="Workshop VTI" img="{workshop}" text="A workshop by students for students" date="30/01/2024"></BlogPost>
    <BlogPost url="scheire-ai" title="Lieven Scheire AI" img="{lieven}" text="" date=""></BlogPost>
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