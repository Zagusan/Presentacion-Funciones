<script>
    import Background from "../lib/Background.svelte";
    import Card from "../lib/Card.svelte";
</script>

<section>
    <section data-auto-animate>
        <Background variant="code">
            <Card vertical variant="alt on-bg" revealId="mainCard">
                <h2>Actividad</h2>
            </Card>
        </Background>
    </section>
    <section data-auto-animate>
        <Background variant="code">
            <Card fullscreen vertical variant="alt on-bg" gap="2rem" revealId="mainCard">
                <h2 style="margin-bottom: auto;">Actividad​</h2>
                <div class="contentLayout">
                    <div class="cardLayout">
                        <Card vertical variant="alt">
                            <img src="/res/users.svg" alt="Icono de dos personas">
                            <p>Hagan parejas</p>
                        </Card>
                        <Card vertical variant="alt">
                            <img src="/res/repeat.svg" alt="Icono de repetición">
                            <p>Tomen turnos adivinando la función del otro</p>
                        </Card>
                        <Card vertical variant="alt">
                            <img src="/res/question-mark.svg" alt="Icono de pregunta">
                            <p>Pueden hacer preguntas de sí o no</p>
                        </Card>
                    </div>
                </div>
            </Card>
        </Background>
    </section>
    <section data-auto-animate>
        <Background variant="code">
            <Card fullscreen vertical variant="alt on-bg" gap="2rem" revealId="mainCard">
                <h2 style="margin-bottom: auto;">Actividad​</h2>
                <div class="contentLayout">
                    <div class="cardLayout">
                        <div></div>
                        <Card vertical variant="alt">
                            <img src="/res/trophy.svg" alt="Icono de trofeo">
                            <p>Gana el primero en adivinar la función (o el que más se acerque)</p>
                        </Card>
                        <div></div>
                    </div>
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

    .cardLayout
    {
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        gap: 2rem;
        margin: 1rem;
        font-size: 2.5rem;
    }
</style>