<script>
    import { Text, Photo } from "./elements";


    export let clase = "presentation";
</script>

<section class={ clase }>
    <Text />
    <Photo />
</section>

<style>
    section {
        display: grid;
        grid-template-columns: 3fr 1fr;
        column-gap: 20px;

        background-color: var(--color-primary);

        max-width: 900px;
        width: 100%;
        height: 400px;
        padding: 0 0 0 5px;
        position: relative;
        
        border-radius: 20px;
        /* border: 2px solid transparent; */
        box-shadow: 0px 3px 6px rgba(0, 0, 0, 0.4);
        transition: width 0.5s ease, height 0.5s ease;
    }
</style>
