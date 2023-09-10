<script>
    import Presentation from "$lib/components/Presentation.svelte";
</script>

<div>
    <Presentation />
    <span>Main</span>
</div>

<style>
    :global(body) {
        margin: 0;
        padding: 0;
        box-sizing: border-box;

        background-color: #222;
    }

    div {
        display: grid;
        justify-items: center;
        column-gap: 20px;

        background-color: white;
        height: 100dvh;
        width: 1200px;
    }

</style>