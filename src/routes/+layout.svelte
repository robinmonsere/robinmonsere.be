<script>
    import Header from './Nav.svelte';
    import './styles.css';
    import '$lib/reset.css'
</script>

<div class="app">
    <main>
        <slot />
    </main>

</div>

<style>
    .app {
        display: flex;
        flex-direction: column;
        min-height: 100vh;
    }






</style>
