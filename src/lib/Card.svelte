<script lang="ts">
    let { 
            children = undefined, 
            fullscreen = false, 
            vertical = false,
            disableAnim = false,
            variant = "",
            revealId = "",
            gap = ""
        } = $props();
</script>

<div class:fullscreen={fullscreen} class="card-root r-stack">
    <div class:vertical={vertical} class="content" style="gap: {gap};">
        {@render children?.()}
    </div>
    <div class="card-bg {variant}" data-id={revealId}></div>
</div>

<style>
    .content,
    .card-bg
    {
        width: 100%;
        height: 100%;
    }

    .content
    {
        position: relative;
        display: flex;
        justify-content: center;
        align-items: center;
        padding: 1rem;
        z-index: 1;
        box-sizing: border-box;
    }

    .card-bg
    {
        background-color: #bad7de99;
        border: 2px solid #bad7de;
        border-radius: 1rem;
        backdrop-filter: blur(4px);
    }

    .card-bg.on-bg
    {
        background-color: #94c5d1cc;
        border: none;
        border-radius: 1rem;
        backdrop-filter: blur(4px);
    }
    .card-bg.on-bg-border
    {
        background-color: #94c5d1cc;
        border: 2px solid #98d7e6;
        border-radius: 1rem;
        backdrop-filter: blur(4px);
    }

    .fullscreen .card-bg.card-bg.on-bg
    {
        border: 2px solid #98d7e6;
    }

    .vertical
    {
        flex-direction: column;
    }

    .horizontal
    {
        flex-direction: row;
    }

    .fullscreen
    {
        width: 100%;
        height: 100%;
    }
</style>