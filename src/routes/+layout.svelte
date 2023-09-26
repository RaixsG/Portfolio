<script>
    import '../styles.css'
    import { backgroundOpacity } from '$lib/stores'
    let isBackgroundActive = false;
    backgroundOpacity.subscribe(value => isBackgroundActive = value);
</script>

<slot />
<div class='background-opacity' class:background-opacity--active={ isBackgroundActive } />

<style>
    .background-opacity {
        position: absolute;
        top: 0;
        left: 0;
        z-index: -1;
        width: 100%;
        height: 100vh;
        background-color: #00000080;
        opacity: 0;
        transition: opacity .4s;
    }
    .background-opacity--active {
        opacity: 1;
        z-index: 0;
    }
</style>