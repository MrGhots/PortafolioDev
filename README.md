
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portafolio Nicolás</title>
    <link rel="stylesheet" href="styles1.css">
    <style>
        /* Estilo para agrandar la letra */
        body {
            font-size: 20px; /* Puedes ajustar este valor según tus preferencias */
            margin-top: -50px; /* Esto es opcional, para ajustar el contenido hacia arriba */
        }

        /* Animación */
        @keyframes scale-up {
            to { scale: 1.5; }
        }

        @keyframes fade-away {
            to { opacity: 0; }
        }

        section {
            view-timeline: --scroll;
        }

        h1 span:first-child {
            animation: fade-away both linear;
            animation-timeline: --scroll;
            animation-range: exit 20% exit 90%;
        }

        h1 span:last-child {
            animation:
                scale-up both ease-in-out,
                fade-away both linear;
            animation-timeline: --scroll;
            animation-range:
                exit 0% exit 100%,
                exit 50% exit 90%;    
        }

        /* basic */
        section {
            position: relative;
            min-height: 100vh;
            display: grid;
            place-items: center;
        }

        header h1 {
    display: none;
}


        h1 span:first-of-type {
            color: #09f;
            font-size: 0.35em;
        }

        section:nth-of-type(1) {
            height: 100vh;
        }

        section:nth-of-type(2) {
            height: 140vh;
        }

        h1 {
            display: grid;
        }

        h2 {
            font-size: clamp(2rem, 5vw + 1rem, 6rem);
            text-align: center;
        }

        section div {
            width: 800px;
            max-width: 100vw;
            padding: 0 1rem;
        }

        :is(h1, h2) {
            font-size: clamp(2.5rem, 7vw + 1rem, 10rem);
            text-align: center;
            line-height: 1;
            position: fixed;
            top: 50%;
            left: 50%;
            margin: 0;
            translate: -50% -50%;
            width: 100%;
        }

        /* reset */
        *, *:after, *:before {
            box-sizing: border-box;
        }

        body {
            background: #000;
            color: white;
            display: grid;
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
            font-weight: 700;
            margin: 0;
            min-height: 100dvh;
            overflow-x: hidden;
            place-items: center;
        }
    </style>
</head>
<body>
    <main>
        <section>
            <div>
                <h1>
                    <span>Portafolio</span>
                    <span>Nicolas Torres</span>
                </h1>
            </div>
        </section>
        <section>
            <h3>Y todo con sólo CSS</h3>
        </section>
    </main>
</body>
</html>
