<script>
    let isOpen = false;
    function toggleModal() {
        isOpen = !isOpen;
    }
</script>

<button
    on:click = { toggleModal }
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
