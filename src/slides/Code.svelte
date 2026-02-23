<script>
    import Background from "../lib/Background.svelte";
    import Card from "../lib/Card.svelte";
</script>

<section>
    <section data-auto-animate>
        <Background variant="code">
            <Card vertical variant="alt on-bg" revealId="mainCard">
                <h2>¡A programar!</h2>
            </Card>
        </Background>
    </section>
    <section data-auto-animate>
        <Background variant="code">
            <Card fullscreen vertical variant="alt on-bg" gap="2rem" revealId="mainCard">
                <h2 style="margin-bottom: auto;">¡A programar!​</h2>
                <div class="contentLayout">
                    <div class="cardLayout">
                        <Card vertical variant="alt">
                            <div style="font-size: 96px;">🤫</div>
                            <p>En secreto, definan una función que utilice <b><code>return</code></b></p>
                        </Card>
                        <Card vertical variant="alt">
                            <code style="font-size: 3rem;"><span>input</span>()</code>
                            <p>Hagan que el programa pida parámetros y se los pase a la función</p>
                        </Card>
                        <Card vertical variant="alt">
                            <code style="font-size: 3rem;"><span>print</span>()</code>
                            <p>Impriman lo que retorna la función para poder ver el resultado</p>
                        </Card>
                    </div>
                </div>
            </Card>
        </Background>
    </section>
    <section data-auto-animate>
        <Background variant="code">
            <Card fullscreen vertical variant="alt on-bg" gap="2rem" revealId="mainCard">
                <h2 style="margin-bottom: auto;">Ejemplo</h2>
                <div class="contentLayout">
                    <pre><code data-trim data-line-numbers class="language-python">
                        def miFuncion(numero):
                            return (2 * numero) + 1

                        entrada = int(input())
                        print(miFuncion(entrada))
                    </code></pre>
                </div>
            </Card>
        </Background>
    </section>
</section>

<style>
    .contentLayout
    {
        flex-grow: 1;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        gap: 2rem;
    }

    .contentLayout pre
    {
        width: min-content;
    }

    .cardLayout
    {
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        gap: 2rem;
        margin: 1rem;
        font-size: 2rem;
    }

    .cardLayout p
    {
        margin-top: auto;
    }

    .cardLayout code span
    {
        color: hsl(80, 76%, 40%);
    }
</style>