<script>
  import Presentation from "$lib/components/presentation/Presentation.svelte";
  import UsedTechnology from "$lib/components/usedTechnology/UsedTechnology.svelte";
  import Github from '$lib/components/github/Github.svelte';
  import Linkedin from '$lib/components/linkedin/Linkedin.svelte';
</script>

<article>
  <Presentation --grid-column="1 / 4" />
  <div class="div_container-used-profile">
      <UsedTechnology />
      <Github />
      <Linkedin />
  </div>
</article>

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

  .div_container-used-profile {
      grid-column: 4;
      position: relative;
      height: 400px;

      display: grid;
      grid-template:
      "usedTechnology  usedTechnology" calc(66.6% - 20px)
      "github linkedin" 33.3% /
      1fr 1fr;
      gap: 20px;
  }

</style>
