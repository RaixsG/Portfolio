<a href="https://github.com/RaixsG">
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
            class="icon icon-tabler icon-tabler-brand-github"
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
                d="M9 19c-4.3 1.4 -4.3 -2.5 -6 -3m12 5v-3.5c0 -1 .1 -1.4 -.5 -2c2.8 -.3 5.5 -1.4 5.5 -6a4.6 4.6 0 0 0 -1.3 -3.2a4.2 4.2 0 0 0 -.1 -3.2s-1.1 -.3 -3.5 1.3a12.3 12.3 0 0 0 -6.2 0c-2.4 -1.6 -3.5 -1.3 -3.5 -1.3a4.2 4.2 0 0 0 -.1 3.2a4.6 4.6 0 0 0 -1.3 3.2c0 4.6 2.7 5.7 5.5 6c-.6 .6 -.6 1.2 -.5 2v3.5"
            />
        </svg>
    </div>
</a>

<style>
    a {
        display: grid;
        grid-area: github;

        width: 100%;
        height: 100%;

        cursor: pointer;

        background-color: var(--color-primary);
        border: none;
        border-radius: 20px;
        box-shadow: 0px 3px 6px rgba(0, 0, 0, 0.4);
        transition: width 0.5s ease, height 0.5s ease;
    }

    a:hover {
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
