<script>
    import Background from "../lib/Background.svelte";
    import Card from "../lib/Card.svelte";
    import StepwiseCode from "../lib/StepwiseCode.svelte";
</script>

<section>
    <section data-auto-animate>
        <Background>
            <Card vertical variant="on-bg" revealId="mainCard">
                <h2>¿Cómo definir una función?</h2>
            </Card>
        </Background>
    </section>
    <section data-auto-animate>
        <Background>
            <Card fullscreen vertical variant="on-bg" gap="2rem" revealId="mainCard">
                <h2 style="margin-bottom: auto;">¿Cómo definir una función?​</h2>
                <StepwiseCode code="def">
                    <p>Palabra clave <b><code>def</code></b></p>
                </StepwiseCode>
            </Card>
        </Background>
    </section>
    <section data-auto-animate>
        <Background>
            <Card fullscreen vertical variant="on-bg" gap="2rem" revealId="mainCard">
                <h2 style="margin-bottom: auto;">¿Cómo definir una función?​</h2>
                <StepwiseCode code="def miFuncion">
                    <p>Nombre de la función</p>
                </StepwiseCode>
            </Card>
        </Background>
    </section>
    <section data-auto-animate>
        <Background>
            <Card fullscreen vertical variant="on-bg" gap="2rem" revealId="mainCard">
                <h2 style="margin-bottom: auto;">¿Cómo definir una función?​</h2>
                <StepwiseCode code="def miFuncion():">
                    <p>Paréntesis y dos puntos</p>
                    <p style="font-size: 32px;">Es posible hacer funciones que no reciban ningún parámetro</p>
                </StepwiseCode>
            </Card>
        </Background>
    </section>
    <section data-auto-animate>
        <Background>
            <Card fullscreen vertical variant="on-bg" gap="2rem" revealId="mainCard">
                <h2 style="margin-bottom: auto;">¿Cómo definir una función?​</h2>
                <StepwiseCode code="def miFuncion(numero1, numero2):">
                    <p>Parámetros</p>
                </StepwiseCode>
            </Card>
        </Background>
    </section>
    <section data-auto-animate>
        <Background>
            <Card fullscreen vertical variant="on-bg" gap="2rem" revealId="mainCard">
                <h2 style="margin-bottom: auto;">¿Cómo definir una función?​</h2>
                <StepwiseCode code="def miFuncion(miNumero, miCadena, miBool, funcion):">
                    <p>Se puede usar <b>cualquier</b> tipo de dato como parámetro</p>
                    <p style="font-size: 32px;">(Inclusive funciones)</p>
                </StepwiseCode>
            </Card>
        </Background>
    </section>
    <section data-auto-animate>
        <Background>
            <Card fullscreen vertical variant="on-bg" gap="2rem" revealId="mainCard">
                <h2 style="margin-bottom: auto;">¿Cómo definir una función?​</h2>
                <StepwiseCode
                    code="def miFuncion(numero1, numero2):
        →→→→pass"
                >
                    <p>Indentación</p>
                    <p style="font-size: 32px;"> (cuatro espacios o una tabulación)</p>
                </StepwiseCode>
            </Card>
        </Background>
    </section>
    <section data-auto-animate>
        <Background>
            <Card fullscreen vertical variant="on-bg" gap="2rem" revealId="mainCard">
                <h2 style="margin-bottom: auto;">¿Cómo definir una función?​</h2>
                <StepwiseCode
                    code='def miFuncion(numero1, numero2):
            mayorOMenor = ""
            # Calcula si numero1 es mayor, menor o igual a numero2
            if numero1 > numero2:
                mayorOMenor = f"{'{numero1}'} es mayor que {'{numero2}'}"
            elif numero1 == numero2:
                mayorOMenor = f"{'{numero1}'} es igual a {'{numero2}'}"
            elif numero1 < numero2:
                mayorOMenor = f"{'{numero1}'} es menor que {'{numero2}'}"'
                >
                    <p><b>Cuerpo</b> de la función</p>
                </StepwiseCode>
            </Card>
        </Background>
    </section>
        <section data-auto-animate>
        <Background>
            <Card fullscreen vertical variant="on-bg" gap="2rem" revealId="mainCard">
                <h2 style="margin-bottom: auto;">¿Cómo definir una función?​</h2>
                <StepwiseCode
                    code='def miFuncion(numero1, numero2):
            mayorOMenor = ""
            # Calcula si numero1 es mayor, menor o igual a numero2
            if numero1 > numero2:
                mayorOMenor = f"{'{numero1}'} es mayor que {'{numero2}'}"
            elif numero1 == numero2:
                mayorOMenor = f"{'{numero1}'} es igual a {'{numero2}'}"
            elif numero1 < numero2:
                mayorOMenor = f"{'{numero1}'} es menor que {'{numero2}'}"
            
            print(mayorOMenor)'
                >
                    <p>Es posible declarar funciones que no retornen ningún valor, conocidas como <b>procedimientos</b></p>
                </StepwiseCode>
            </Card>
        </Background>
    </section>
    <section data-auto-animate>
        <Background>
            <Card fullscreen vertical variant="on-bg" gap="2rem" revealId="mainCard">
                <h2 style="margin-bottom: auto;">¿Cómo definir una función?​</h2>
                <StepwiseCode
                    code='def miFuncion(numero1, numero2):
            mayorOMenor = ""
            # Calcula si numero1 es mayor, menor o igual a numero2
            if numero1 > numero2:
                mayorOMenor = f"{'{numero1}'} es mayor que {'{numero2}'}"
            elif numero1 == numero2:
                mayorOMenor = f"{'{numero1}'} es igual a {'{numero2}'}"
            elif numero1 < numero2:
                mayorOMenor = f"{'{numero1}'} es menor que {'{numero2}'}"
            
            return mayorOMenor'
                >
                    <p>Alternativamente, se puede devolver un valor con <b><code>return</code></b></p>
                </StepwiseCode>
            </Card>
        </Background>
    </section>
    <section data-auto-animate>
        <Background>
            <Card fullscreen vertical variant="on-bg" gap="2rem" revealId="mainCard">
                <h2 style="margin-bottom: auto;">¿Cómo definir una función?​</h2>
                <StepwiseCode
                    code='print(miFuncion(3, 2)) # Imprime "3 es mayor que 2"
        print(miFuncion(5, 5)) # Imprime "5 es igual a 5"
        print(miFuncion(1, 9)) # Imprime "1 es menor que 9"'
                >
                    <p>Así es como se usaría la función</p>
                </StepwiseCode>
            </Card>
        </Background>
    </section>
</section>