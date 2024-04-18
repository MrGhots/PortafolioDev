
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portafolio Nicolas</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
    <link rel="stylesheet" href="styles.css">
    <style>
        /* Tu CSS modificado */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f0f0;
        }
        header {
            background-color: #333;
            color: #fff;
            padding: 40px 0;
            text-align: center;
        }
        header h1 {
            margin: 0;
        }
        nav {
            display: flex;
            justify-content: center;
            background-color: #444;
            padding: 10px 0;
        }
        nav a {
            color: #fff;
            text-decoration: none;
            padding: 10px 20px;
        }
        .initial-section {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100vh; /* Ajusta la altura para que abarque toda la pantalla */
            background-color: #666; /* Color de fondo gris */
            z-index: 1000; /* Asegura que esté encima de todas las demás secciones */
            opacity: 1; /* Asegura que sea visible al inicio */
            transition: opacity 1s ease-in-out; /* Agrega una transición suave */
        }

        .welcome-panel {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100vh;
            background-color: rgba(0, 0, 0, 0.7); /* Fondo oscuro semitransparente */
            z-index: 1000;
            display: flex;
            justify-content: center;
            align-items: center;
            opacity: 1; /* Inicialmente visible */
            transition: opacity 1s ease-in-out; /* Transición de opacidad */
        }

        .welcome-message {
            text-align: center;
            color: #fff;
            padding: 20px;
            max-width: 80%;
        }

        .welcome-message h2 {
            font-size: 2em;
            margin-bottom: 10px;
        }

        .welcome-message p {
            font-size: 1.2em;
            margin: 0;
        }

        .section-wrapper {
            background-color: #f9f9f9; /* Color de fondo del rectángulo blanco */
            border-radius: 10px; /* Redondear los bordes */
            padding: 40px 20px; /* Ajustar el padding para cambiar la altura */
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1); /* Agregar sombra */
            margin-bottom: 40px; /* Espacio entre las secciones */
        }
        section {
            padding: 40px;
            margin: auto;
            max-width: 1200px;
        }
        #sobre-mi {
            text-align: center; /* Centrar el contenido horizontalmente */
             font-family: Arial, sans-serif; /* Utiliza la tipografía Arial */
            margin-top: 40px; /* Agregar un margen superior para separarla del contenido anterior */
        }
        .profile {
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 40px;
        }
.profile img {
    border-radius: 50%;
    width: 300px; /* Ajusta el ancho de la imagen */
    height: 300px; /* Ajusta la altura de la imagen */
    margin-right: 20px;
    position: relative;
    overflow: hidden;

        }
        .profile-text {
            max-width: 600px;
            text-align: center;
        }
        .skills li {
            margin: 10px;
            padding: 10px 20px;
            background-color: #666;
            color: #fff;
            border-radius: 20px;
            transition: background-color 0.3s, transform 0.3s; /* Agregar transiciones suaves */
        }

        .skills li:hover {
            background-color: #555; /* Cambiar el color de fondo al pasar el mouse */
            transform: scale(1.05); /* Aumentar ligeramente el tamaño al pasar el mouse */
            cursor: auto; /* Mantener el cursor normal */
        }

        .skills {
            margin-bottom: 40px;
        }
        .skills ul {
            list-style: none;
            padding: 0;
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
        }
        .skills li {
            margin: 10px;
            padding: 10px 20px;
            background-color: #666;
            color: #fff;
            border-radius: 20px;
        }

        .experience ul {
            list-style-type: none; /* Eliminar los puntos de la lista */
            padding: 0; /* Eliminar el padding para ajustar los elementos al texto */
        }

        .experience li {
            text-align: center; /* Alinear el texto a la izquierda */
            margin-left: -20px; /* Reducir el margen izquierdo para acercar los puntos al texto */
        }

        .experience {
            margin-bottom: 40px;
            background-color: #f9f9f9; /* Agregar un color de fondo */
            border-radius: 10px; /* Redondear los bordes */
            padding: 40px 20px; /* Agregar espacio interno */
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1); /* Agregar sombra */
        }

        .experience h2 {
            text-align: center; /* Centrar el título */
            margin-bottom: 20px; /* Agregar espacio debajo del título */
        }

        .projects {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-around;
        }

        .project {
            width: 300px;
            margin: 20px;
            border: 1px solid #ccc;
            border-radius: 5px;
            padding: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            background-color: #fff;
        }
        #contacto {
            text-align: center; /* Centrar el contenido horizontalmente */
            margin-top: 40px; /* Agregar un margen superior para separarla del contenido anterior */
        }
        #proyectos {
            text-align: center; /* Centrar el contenido horizontalmente */
            margin-top: 40px; /* Agregar un margen superior para separarla del contenido anterior */
        }
        #habilidades {
            text-align: center; /* Centrar el contenido horizontalmente */
            margin-top: 40px; /* Agregar un margen superior para separarla del contenido anterior */
        }
        #experiencia {
            text-align: center; /* Centrar el contenido horizontalmente */
            margin-top: 40px; /* Agregar un margen superior para separarla del contenido anterior */
        }

        .project img {
            width: 100%;
            border-radius: 5px;
            margin-bottom: 10px;
        }
        footer {
            background-color: #333;
            color: #fff;
            text-align: center;
            padding: 20px;
        }
        .social-icons {
            text-align: center;
        }
        .social-icons a {
            color: #333;
            text-decoration: none;
            font-size: 24px;
            margin: 0 10px;
            transition: color 0.3s ease;
        }

        .social-icons a:hover {
            color: #666;
        }
        .profile img {
    border-radius: 50%;
    width: 300px; /* Ajusta el ancho de la imagen */
    height: 300px; /* Ajusta la altura de la imagen */
    margin-right: 20px;
}

.profile {
    display: flex;
    align-items: center;
    justify-content: center;
    margin-bottom: 40px;
    position: relative; /* Agrega posición relativa para los pseudoelementos */
}


.profile img::after {
    content: "";
    position: absolute;
    top: 50%; /* Posiciona el degradado en la mitad vertical de la imagen */
    left: 0;
    transform: translateY(-50%); /* Centra verticalmente el degradado */
    width: 100%;
    height: 50px; /* Altura del degradado */
    background: linear-gradient(to bottom, rgba(255,255,255,1), rgba(255,255,255,0)); /* Degradado de blanco opaco a blanco transparente */
}
}

.profile::before {
    left: -20px; /* Coloca el elemento decorativo a la izquierda */
}

.profile::after {
    right: -20px; /* Coloca el elemento decorativo a la derecha */
}

.profile {
    background-image: linear-gradient(to top, #ffffff, rgba(255, 255, 255, 0)); /* Degradado de blanco a transparente */
}

        @media screen and (max-width: 768px) 
            .section {
                padding: 40px 20px; /* Reducir el padding horizontal para dar más espacio al contenido */
             }
             .profile {
                flex-direction: column;
            }
            .profile img {
                mask-image: linear-gradient(
                white 80%
                trasparent
                )
                width: 150px; /* Ajustar el tamaño de la imagen según sea necesario */
                margin-right: 0;
                margin-bottom: 10px; /* Reducir el margen inferior */
            }
            nav {
                display: block; /* Cambiar a una lista vertical en dispositivos móviles */
            }
            .projects {
                justify-content: center; /* Centrar los proyectos horizontalmente */
            }
            section, .profile, .experience, .skills, .projects, .social-icons {
                max-width: 100%; /* Ajustar el ancho máximo al 100% en dispositivos móviles */
            }
               /* Definir la fuente Showcard Gothic */
/* Definir la fuente Showcard Gothic */
@font-face 
    font-family: font-family: Arial, sans-serif;
    src: url('') format('truetype');
}

/* Aplicar la fuente Showcard Gothic solo al h1 */
header h1 {
    font-family: 'font-family: Arial, sans-serif', sans-serif;
}



    </style>
</head>
<body>
    <div class="initial-section">
        <div class="welcome-panel">
            <div class="welcome-message">
                <h2>Bienvenido a mi Portafolio</h2>
                <p>Gracias por visitar mi sitio web. Aquí encontrarás información sobre mí y mis proyectos.</p>
            </div>
        </div>
    </div>

    <header>
    <h1><strong>Nicolás Torres Molina</strong></h1>
    </header>
    <nav>
        <a href="#sobre-mi">Sobre Mí</a>
        <a href="#experiencia">Experiencia</a>
        <a href="#habilidades">Habilidades</a>
        <a href="#proyectos">Proyectos</a>
        <a href="#contacto">Contacto</a>
    </nav>
    <section id="sobre-mi" class="section-wrapper">
        <h2>Sobre Mí</h2>
        <div class="profile">
            <img src="https://media.discordapp.net/attachments/1198362548647514309/1230351297824292864/Background_Eraser.png?ex=663300f0&is=66208bf0&hm=203f8dd5c9841b043104b27c53ca54f69ad68a20bcbd1d2d2a8690da418b0e74&=&format=webp&quality=lossless&width=447&height=468" alt="Tu Foto">
            <div class="profile-text">
                <p>¡Hola👋! Soy ,<strong>Nicolás</strong> joven un apasionado por la programación con años de experiencia en el desarrollo web. Me encanta crear proyectos innovadores y aprender nuevas tecnologías. Estoy comprometido a proporcionar soluciones de alta calidad y mejorar constantemente mis habilidades.</p>
            </div>
        </div>
    </section>
    <section id="experiencia" class="section-wrapper experience">
        <h2>Experiencia</h2>
        <p><strong>Tengo Experiencia En:</strong></p>
        <ul>
            <li>Desarrollo Frontend (HTML, CSS, JavaScript)</li>
            <li>Desarrollo Backend (Python )</li>
            <li>Bases de Datos (SQL, MongoDB)</li>
            <li>Frameworks y Librerías (React, Vue.js)</li>
            <!-- Agregar más según sea necesario -->
        </ul>
    </section>
    <section id="habilidades" class="section-wrapper skills">
        <h2>Habilidades</h2>
        <ul>
            <li>HTML</li>
            <li>CSS</li>
            <li>JavaScript</li>
            <li>Python</li>
            <li>Diseño Grafico</li>
            <li>Comunicación</li>
            <!-- Agregar más según sea necesario -->
        </ul>
    </section>
    <section id="proyectos" class="section-wrapper">
        <h2>Proyectos</h2>
        <div class="projects">
            <div class="project">
                <img src="proyecto1.jpg" alt="Proyecto 1">
                <h3>Login</h3>
                <p>Login llamativo animado.</p>
            </div>
            <div class="project">
                <img src="proyecto2.jpg" alt="Proyecto 2">
                <h3>Calculadora</h3>
                <p>Calculadora funcional estilo iOS</p>
            </div>
            <!-- Agregar más proyectos según sea necesario -->
        </div>
    </section>
    <section id="contacto" class="section-wrapper">
        <h2>Contacto</h2>
        <div class="social-icons">
            <a href="https://www.instagram.com/nico_tmrx_?igshid=MWs2eGtkNHZreHQ4ag%3D%3D&utm_source=qr"><i class="fab fa-instagram"></i></a>
            <a href="https://www.linkedin.com/"><i class="fab fa-linkedin"></i></a>
            <a href="https://wa.me/3125534086"><i class="fab fa-whatsapp"></i></a>
            <a href="mailto:torresmolinanicolas838@gmail.com"><i class="fas fa-envelope"></i></a>
        </div>
    </section>
    <footer>
        &copy; 2024 DevNico
    </footer>
    <script>
        // JavaScript para desplazamiento suave al hacer clic en los enlaces del menú
        document.addEventListener('DOMContentLoaded', function() {
            // Espera a que se cargue completamente el contenido HTML

            // Obtén la sección gris inicial
            const initialSection = document.querySelector('.initial-section');

            // Espera un corto tiempo antes de ocultar la sección inicial
            setTimeout(function() {
                // Reduce la opacidad de la sección gris
                initialSection.style.opacity = '0';

                // Espera a que termine la animación de opacidad
                setTimeout(function() {
                    // Oculta la sección gris
                    initialSection.style.display = 'none';
                }, 2000); // 2000ms (2 segundo) es la duración de la animación definida en el CSS

                // Muestra el contenido principal después de la animación
                document.body.style.overflow = 'auto'; // Permite desplazamiento nuevamente
            }, 5000); // 5000ms (5 segundos) es el tiempo antes de ocultar la sección inicial


            // Seleccionar todos los enlaces del menú de navegación
            const links = document.querySelectorAll('nav a');

            // Agregar un event listener a cada enlace
            links.forEach(link => {
                link.addEventListener('click', smoothScroll);
            });

            // Función para el desplazamiento suave
            function smoothScroll(event) {
                // Prevenir el comportamiento predeterminado del enlace
                event.preventDefault();

                // Obtener el ID del objetivo del enlace
                const targetId = this.getAttribute('href').substring(1);

                // Obtener el elemento de destino
                const targetElement = document.getElementById(targetId);

                // Calcular la distancia al elemento de destino
                const targetPosition = targetElement.offsetTop;

                // Calcular la posición actual de la página
                let startPosition = window.pageYOffset;

                // Duración de la animación en milisegundos
                const duration = 7000;

                // Función de animación
                function animation(currentTime) {
                    const elapsedTime = currentTime - startTime;
                    const progress = Math.min(elapsedTime / duration, 1);
                    const ease = easeInOutCubic(progress);
                    window.scrollTo(0, startPosition + ((targetPosition - startPosition) * ease));

                    if (elapsedTime < duration) {
                        requestAnimationFrame(animation);
                    }
                }

                // Calcular el tiempo de inicio de la animación
                const startTime = performance.now();

                // Iniciar la animación
                requestAnimationFrame(animation);
            }

            // Función de aceleración suave
            function easeInOutCubic(t) {
                return t < 0.5 ? 4 * t * t * t : (t - 1) * (2 * t - 2) * (2 * t - 2) + 1;
            }
        });
    </script>
</body>
</html>
