<script>
    export let name;
</script>

<div>
    <p>{name}</p>
</div>

<style>

    p {
        color: var(--color-theme-1);
        display: inline-block;
        border-radius: 2rem;
        font-size: 0.8rem;
        font-weight: bold;
    }
    div {
        display: inline-block;
        padding: 0.5rem;
        border-radius: 2rem;
        background: var(--color-theme-2);
    }
</style>