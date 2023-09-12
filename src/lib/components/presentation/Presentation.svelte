<script>
    import { Text, Photo } from './elements'
    let isOpen = false;
    function toggleModal() {
        isOpen = !isOpen;
    }
</script>

<button
    on:click = { toggleModal }
    class:expanded = { isOpen }
>
    <Text />
    <Photo />
</button>

<style>
    button {
        max-width: 100%;
        width: 600px;
        background-color: var(--color-primary);
        padding: 5px;
        border-radius: 20px;
        border: 2px solid transparent;
        box-shadow: 0px 3px 6px rgba(0, 0, 0, 0.4);
        cursor: pointer;
        transition: width 0.5s ease, height 0.5s ease;
    }
    /* isOpen -> True */
    .expanded {
    position: absolute;
    width: 800px;
    height: 400px;
    }
</style>