<script>
    import BlogNav from "./BlogNav.svelte";
    import './../styles.css';
    import '$lib/reset.css'
</script>


<div class="app">
    <BlogNav></BlogNav>
    <main>
        <slot />
    </main>
</div>

<style>

    .app {
        display: flex;
        flex-direction: column;
        margin: 0 15vw 5rem 15vw;
        height: 100%;
    }

</style>