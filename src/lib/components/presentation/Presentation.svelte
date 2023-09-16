<script>
    import { Text, Photo } from "./elements";
</script>

<section>
    <Text />
    <Photo />
</section>

<style>
    section {
        display: grid;
        grid-template-columns: 3fr 1fr;
        grid-column: var(--grid-column);
        column-gap: 20px;

        max-width: 900px;
        width: 100%;
        height: 400px;
        padding: 0 0 0 5px;
        overflow: hidden; /*Usar cuando se hace mas pequeño*/
        position: relative;
        
        background-color: var(--color-primary);
        
        border-radius: 20px;
        /* border: 2px solid transparent; */
        box-shadow: 0px 3px 6px rgba(0, 0, 0, 0.4);
        transition: width 0.5s ease, height 0.5s ease;
    }
</style>
