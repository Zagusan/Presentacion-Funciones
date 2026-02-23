<script>
    import Background from "../lib/Background.svelte";
    import Card from "../lib/Card.svelte";
</script>

<section>
    <section data-auto-animate>
        <Background>
            <Card vertical variant="on-bg" revealId="mainCard">
                <h2>¿Qué es una función?</h2>
            </Card>
        </Background>
    </section>
    <section data-auto-animate>
        <Background>
            <Card fullscreen vertical variant="on-bg" gap="2rem" revealId="mainCard">
                <h2 style="margin-bottom: auto;">¿Qué es una función?​</h2>
                <div class="contentLayout">
                    <h4>Hay varias formas de describir qué son</h4>
                    <div class="cardLayout">
                        <Card vertical>
                            <div class="relation">
                                <div style="color: #000080;">x</div>
                                <img src="/res/arrow-big-right.svg" alt="Flecha que apunta hacia la derecha">
                                <div style="color: #0f52ba;">y</div>
                            </div>
                            <p>Una relación entre dos valores</p>
                        </Card>
                        <Card vertical>
                            <img style="width: 60%; margin: 0;" src="/res/packaging-closing-machine.svg" alt="Máquina empaquetadora de cajas">
                            <p>Una máquina con entradas y salidas</p>
                            <a class="imgCredit" href="https://www.vecteezy.com/vector-art/4578887-packaging-closing-machine">Imagen por Hasan As ari</a>
                        </Card>
                        <Card vertical>
                            <img style="width: 55%; margin: 0; margin: 20px;" src="/res/laptop-code-block.svg" alt="Laptop mostrando un bloque de código abstracto">
                            <p>Un bloque de código reutilizable</p>
                            <a class="imgCredit" href="https://www.vecteezy.com/vector-art/16321787-meta-description-vector-icon-design">Imagen por Muhammad Usman</a>
                        </Card>
                    </div>
                </div>
            </Card>
        </Background>
    </section>
    <section data-auto-animate>
        <Background>
            <Card fullscreen vertical variant="on-bg" gap="2rem" revealId="mainCard">
                <h2 style="margin-bottom: auto;">Funciones comunes</h2>
                <div class="contentLayout">
                    <Card vertical>
                        <ul>
                            <li><code>print()</code></li>
                            <li><code>input()</code></li>
                            <li><code>max()</code></li>
                            <li><code>min()</code></li>
                            <li><code>sum()</code></li>
                            <li><code>range()</code></li>
                            <li><code>str()</code></li>
                        </ul>
                    </Card>
                </div>
            </Card>
        </Background>
    </section>
</section>

<style>
    @font-face
    {
        font-family: "Chicle";
        src: url("/res/Chicle-Regular.ttf");
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

    .relation
    {
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        gap: 0.5rem;
        padding: 0.5rem;
    }

    .relation img
    {
        height: 100%;
        margin: 0;
    }

    .relation div
    {
        height: 100%;
        font-size: 4cqi;
        font-family: "Chicle";
        text-align: center;
    }

    .imgCredit
    {
        font-size: 1.25rem;
    }
</style>