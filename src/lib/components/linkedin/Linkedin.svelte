<script>
    const openNewTab = () => {
        window.open(
            "https://www.linkedin.com/in/alessyo-jhardell-linares-vargas-3a8461264/",
            "_blank"
        );
    };
</script>

<button on:click={openNewTab}>
    <div>
        <svg
            xmlns="http://www.w3.org/2000/svg"
            class="icon icon-tabler icon-tabler-external-link"
            width="20px"
            height="20px"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="var(--color-secondary)"
            fill="none"
            stroke-linecap="round"
            stroke-linejoin="round"
        >
            <path stroke="none" d="M0 0h24v24H0z" fill="none" />
            <path
                d="M12 6h-6a2 2 0 0 0 -2 2v10a2 2 0 0 0 2 2h10a2 2 0 0 0 2 -2v-6"
            />
            <path d="M11 13l9 -9" />
            <path d="M15 4h5v5" />
        </svg>
        <svg
            xmlns="http://www.w3.org/2000/svg"
            class="icon icon-tabler icon-tabler-brand-linkedin"
            width="80"
            height="80"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="#222"
            fill="none"
            stroke-linecap="round"
            stroke-linejoin="round"
        >
            <path stroke="none" d="M0 0h24v24H0z" fill="none" />
            <path
                d="M4 4m0 2a2 2 0 0 1 2 -2h12a2 2 0 0 1 2 2v12a2 2 0 0 1 -2 2h-12a2 2 0 0 1 -2 -2z"
            />
            <path d="M8 11l0 5" />
            <path d="M8 8l0 .01" />
            <path d="M12 16l0 -5" />
            <path d="M16 16v-3a2 2 0 0 0 -4 0" />
        </svg>
    </div>
</button>

<style>
    button {
        z-index: 1;
        display: grid;
        grid-area: linkedin;

        width: 100%;
        height: 100%;

        cursor: pointer;

        background-color: var(--color-primary);
        border: none;
        border-radius: 20px;
        box-shadow: 0px 3px 6px rgba(0, 0, 0, 0.4);
        transition: width 0.5s ease, height 0.5s ease;
    }

    button:hover {
        filter: saturate(1.5);
    }

    div {
        position: relative;
        display: grid;
        place-items: center;
    }

    .icon-tabler-external-link {
        position: absolute;
        top: 10px;
        right: -45px;
        fill: transparent;
    }
</style>
