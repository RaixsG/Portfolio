<script>
    let isOpen = false;
    /**
     * @type {HTMLAnchorElement}
     */
    let modalUsedTechnology;

    function toggleModal() {
        isOpen = !isOpen;
        if (isOpen) {
            modalUsedTechnology.style.width = "800px";
            modalUsedTechnology.style.height = "400px";
            modalUsedTechnology.style.position = 'absolute';
        }
    }
</script>

<a
    href = "usedTechnology"
    data-sveltekit-noscroll
    on:click = { toggleModal }
    bind:this={ modalUsedTechnology }
    class:expanded = { isOpen }
>
    <div>
        <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Odio atque
            qui, sed, pariatur voluptas non laborum deleniti numquam aliquid
            provident quia deserunt quidem. Quo, facere tenetur illo molestiae
            quas ex.
        </p>
    </div>
</a>

<style>
    a {
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
        width: 800px;
        height: 400px;
        transition: max-width 0.5s ease;
        position: absolute;
    }

</style>
