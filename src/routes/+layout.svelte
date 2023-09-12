<script>
    import '../styles.css'
    import Presentation from "$lib/components/presentation/Presentation.svelte";
    import UsedTechnology from "$lib/components/usedTechnology/UsedTechnology.svelte";
</script>

<article>
    <Presentation />
    <UsedTechnology />
</article>
<slot />

<style>
    article {
        max-width: 100%;
        width: 1200px;
        margin: auto;
        margin-top: 25px;

        display: grid;
        justify-content: center;
        grid-template-columns: 1fr auto minmax(20px, auto);
        column-gap: 20px;
    }
</style>
