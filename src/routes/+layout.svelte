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

        display: grid;
        justify-content: center;
        grid-template-columns: repeat(4, 1fr);
        column-gap: 20px;
    }

    .presentation {
        grid-column: 1 / 3;
    }

    .usedTechnology {
        grid-column: 3 / 5;
    }

</style>
