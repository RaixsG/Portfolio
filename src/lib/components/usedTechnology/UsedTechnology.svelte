<script>
    import { technologies } from '$lib/constants'
    import { backgroundOpacity } from '$lib/stores'
    const switchBackgroundOpacity = () => backgroundOpacity.update(old => !old);
</script>

<!-- svelte-ignore a11y-no-static-element-interactions -->
<section
    on:mouseenter={ switchBackgroundOpacity }
    on:mouseleave={ switchBackgroundOpacity }
>
    {#each technologies as technologie}
    <span>
        <svg
            xmlns="http://www.w3.org/2000/svg"
            class={`icon icon-tabler icon-tabler-brand-${technologie}`}
            width="75"
            height="75"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="#222"
            fill="none"
            stroke-linecap="round"
            stroke-linejoin="round"
        >
            <path stroke="none" d="M0 0h24v24H0z" fill="none" />
            {#each technologie.paths as path}
                <path d={path} />
            {/each}
        </svg>
    </span>
    {/each}
</section>

<style>
    section {
        position: absolute;
        top: 0;
        right: 0;
        z-index: 1;

        display: grid;
        grid-template-columns: repeat(auto-fill, minmax(100px, 1fr));
        grid-area: usedTechnology;

        width: 100%;
        height: 100%;
        padding: 5px;

        background-color: var(--color-primary);

        border-radius: 20px;
        box-shadow: 0px 3px 6px rgba(0, 0, 0, 0.4);
        transition: width 0.5s ease-in-out, height 0.5s ease-in-out 0.5s;
        overflow: hidden;
    }

    section:hover {
        width: 150%;
        height: 150%;
        grid-template-columns: repeat(auto-fill, minmax(100px, 1fr));
        overflow: hidden;
    }

    span {
        width: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        transition: all 0.5s ease;
    }
</style>
