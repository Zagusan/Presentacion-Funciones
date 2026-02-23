<script>
    import Background from "../lib/Background.svelte";
    import Card from "../lib/Card.svelte";
    import RevealLogo from "/reveal-black-text.svg";
    import LucideLogo from "/lucide-logo-light.svg";
    import SvelteLogo from "/svelte-horizontal.svg";
    import Clockwork from "/clockwork.jpg";
    import Code from "/codigo-python-c.jpg";
</script>

<section>
    <section data-auto-animate>
        <Background variant="credits">
            <Card vertical variant="on-bg" revealId="mainCard">
                <h2>Créditos</h2>
            </Card>
        </Background>
    </section>
    <section data-auto-animate>
        <Background variant="credits">
            <Card vertical variant="on-bg-border" gap="2rem" revealId="mainCard">
                <h2 style="margin-bottom: auto;">Créditos​</h2>
                <div class="contentLayout">
                    <div class="cardLayout">
                        <Card vertical>
                            <img src={RevealLogo} alt="Logotipo de Reveal.js">
                            <a href="https://github.com/hakimel/reveal.js/blob/master/LICENSE">Ver licencia</a>
                        </Card>
                        <Card vertical>
                            <div class="horizontal" style="justify-content: center; align-items: center; gap: 1.25rem; width: 100%; height: 100%;">
                                <img style="height: 65%;" src={LucideLogo} alt="Logotipo de Lucide">
                                <h3>Lucide</h3>
                            </div>
                            <a href="https://lucide.dev/license">Ver licencia</a>
                        </Card>
                        <Card vertical>
                            <img src={SvelteLogo} alt="Logotipo de Svelte">
                            <a href="https://github.com/sveltejs/svelte/blob/main/LICENSE.md">Ver licencia</a>
                        </Card>
                    </div>
                </div>
            </Card>
        </Background>
    </section>
    <section data-auto-animate>
        <Background variant="credits">
            <Card vertical variant="on-bg-border" gap="2rem" revealId="mainCard">
                <h2 style="margin-bottom: auto;">Recursos</h2>
                <div class="contentLayout">
                    <div class="cardLayout">
                        <Card vertical>
                            <img style="border-radius: 1rem; height: 200px" src={Clockwork} alt="Interior de un reloj mecánico">
                            <a href="https://www.freepik.com/free-photo/clockwork_3011934.html">Imagen creada por rawpixel.com</a>
                        </Card>
                        <Card vertical>
                            <img style="border-radius: 1rem; height: 200px;" src={Code} alt="Código de Python en una pantalla">
                            <a href="https://pixabay.com/photos/data-computer-programming-codes-5606639/">Imagen creada por suixin390</a>
                        </Card>
                        <Card vertical>
                            <h1 style="color: #0f52ba; font-family: 'Chicle';">Tipografía<br>Chicle</h1>
                            <a href="https://fonts.google.com/specimen/Chicle/license">Ver licencia</a>
                        </Card>
                    </div>
                </div>
            </Card>
        </Background>
    </section>
</section>

<style>
    @font-face
    {
        font-family: "Chicle";
        src: url("/Chicle-Regular.ttf");
    }

    .contentLayout
    {
        flex-grow: 1;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        gap: 2rem;
    }

    .cardLayout
    {
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        gap: 2rem;
        margin: 1rem;
        font-size: 2.5rem;
    }

    .cardLayout img
    {
        height: 90%;
        object-fit: cover;
    }

    .horizontal
    {
        display: flex;
        flex-direction: row;
        gap: 4rem;
    }

    a
    {
        color: #222 !important;
    }
</style>