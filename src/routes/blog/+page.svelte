<script>
    import lieven from '$lib/images/LievenAI.png'
    import starbase from '$lib/images/starbase.jpg'
    import workshop from '$lib/images/workshop1.jpg'
    import usa from '$lib/images/usa.jpg';
    import incaso from '$lib/images/incaso.jpg';
    import porftolio from '$lib/images/porfolio.png';
    import flutter from '$lib/images/flutter.png';
    import BlogPost from "./BlogPost.svelte";
</script>

<div>
    <h1>Robin Monseré's <span>blog</span></h1>
</div>
<section id="blogPosts">
    <BlogPost url="flutter-meetup" title="The Flutter Belgium Meetup" img="{flutter}" text="An event organised by Flutter Belgium" date="15/05/2024"></BlogPost>
    <BlogPost url="usa" title="International study in the USA" img="{usa}" text="" date="15/08/2023 - 6/01/2024"></BlogPost>
    <BlogPost url="ift-2" title="Starship IFT-2" img="{starbase}" text="Witnessing the second test flight of the largest rocket ever made" date="18/11/2023"></BlogPost>
    <BlogPost url="workshop-vti" title="Workshop @ VTI Izegem" img="{workshop}" text="A workshop by students for students" date="30/01/2024"></BlogPost>
    <BlogPost url="scheire-ai" title="Lieven Scheire AI" img="{lieven}" text="Lieven Scheire talks about AI" date="02/02/2024"></BlogPost>
    <BlogPost url="portfolio" title="Portfolio" img="{porftolio}" text="Learn how I created this portfolio and blog!" date="22/02/2024"></BlogPost>
    <BlogPost url="incaso" title="Incaso 2023" img="{incaso}" text="International project in Rijeka, Croatia" date="12/02/23 - 19/02/23"></BlogPost>
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


    @media screen and (max-width: 1000px) {
        #blogPosts {
            width: 100%;
            flex-direction: column;
        }
    }
</style>