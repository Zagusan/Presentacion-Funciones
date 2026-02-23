<script lang="ts">
    let {
        children = undefined,
        variant = "" // Me dió pereza cambiar todo el código solo para poner otra imagen de fondo zzz
        } = $props();
</script>

<div class="bg {variant}">
    {@render children?.()}
</div>

<style>
    .bg
    {
        width: 100%;
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        background-image: url(/res/clockwork.jpg);
        background-color: rgba(0, 165, 255, 0.5);
        background-blend-mode: multiply;
        background-size: cover;
        padding: 2rem;
        box-sizing: border-box;
    }

    .bg.code
    {
        background-image: url(/res/codigo-python-c.jpg);
        background-color: transparent;
    }

    .bg.credits
    {
        background-image: linear-gradient(to bottom, hsl(192, 40%, 40%), hsl(192, 30%, 20%));
        background-color: transparent;
    }
</style>