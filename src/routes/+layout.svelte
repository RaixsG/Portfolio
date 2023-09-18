<script>
    import '../styles.css'
    import Presentation from "$lib/components/presentation/Presentation.svelte";
    import UsedTechnology from "$lib/components/usedTechnology/UsedTechnology.svelte";
    import Github from '$lib/components/github/Github.svelte';
    import Linkedin from '$lib/components/linkedin/Linkedin.svelte';
</script>

<article>
    <Presentation --grid-column="1 / 4" />
    <div class="div_container-used-perfil">
        <UsedTechnology />
        <Github />
        <Linkedin />
    </div>
</article>
<slot />

<style>
    article {
        position: relative;
        max-width: 100%;
        width: 1200px;
        margin: 0 auto;
        margin-top: 50px;

        display: grid;
        grid-template-columns: repeat(4, 1fr);
        grid-auto-rows: 200px;
        column-gap: 20px;
    }

    .div_container-used-perfil {
        grid-column: 4 / 5;
        position: relative;

        height: 400px;
        display: grid;
        grid-template-areas: "usedTechnology  usedTechnology"
                              "github linkedin";
        column-gap: 20px;
        row-gap: 20px;
    }

</style>
