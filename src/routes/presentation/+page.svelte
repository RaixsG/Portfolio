<script>
  import { goto } from "$app/navigation"
  const exit = () => goto("/");
</script>

<section>
  <button on:click={ exit }>x</button>
  <h1>Presentación</h1>
</section>

<style>
  section {
    width: 80%;
    max-width: 768px;
    height: 50vh;
    background-color: var(--gray);
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translateY(-50%) translateX(-50%);
  }
  button {
    background-color: var(--color-primary);
    position: absolute;
    width: 1.5rem;
    height: 1.5rem;
    top: 0;
    right: 0;
    margin: 1rem;
  }
</style>