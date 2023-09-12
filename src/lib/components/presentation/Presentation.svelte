<script>
    import { Text, Photo } from './elements'

</script>

<a href="presentation" data-sveltekit-noscroll>
    <Text />
    <Photo />
</a>

<style>
    a {
        background-color: var(--color-primary);
        border-radius: 20px;
        padding: 5px;
        box-shadow: 0px 3px 6px rgba(0, 0, 0, 0.4);

        border: 2px solid transparent;
        cursor: pointer;
    }

    a {
        max-width: 100%;
        width: 600px;
    }
</style>