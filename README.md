
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portafolio Nicolas</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
    <style>
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
        section {
            padding: 40px;
            margin: auto;
            max-width: 1200px;
        }
        .profile {
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 40px;
        }
        .profile img {
            border-radius: 50%;
            width: 200px;
            height: 200px;
            margin-right: 20px;
        }
        .profile-text {
            max-width: 600px;
            text-align: center;
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
        .experience {
            margin-bottom: 40px;
        }
        .experience h2 {
            text-align: center;
            margin-bottom: 20px;
        }
        .experience p {
            text-align: justify;
            line-height: 1.6;
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
    @media screen and (max-width: 768px) {
    section {
        padding: 40px 20px; /* Reducir el padding horizontal para dar más espacio al contenido */
    }
    .profile {
        flex-direction: column;
    }
    .profile img {
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
}


    </style>
</head>
<body>
    <header>
        <h1>Nicolás Torres Molina</h1>
    </header>
    <nav>
        <a href="#sobre-mi">Sobre Mí</a>
        <a href="#experiencia">Experiencia</a>
        <a href="#habilidades">Habilidades</a>
        <a href="#proyectos">Proyectos</a>
        <a href="#contacto">Contacto</a>
    </nav>
    <section id="sobre-mi">
        <h2>Sobre Mí</h2>
        <div class="profile">
            <img src="tu_foto.jpg" alt="Tu Foto">
            <div class="profile-text">
            <p>¡Hola👋! Soy ,<strong>Nicolás</strong>strong> joven un apasionado por la programación con años de experiencia en el desarrollo web. Me encanta crear proyectos innovadores y aprender nuevas tecnologías. Estoy comprometido a proporcionar soluciones de alta calidad y mejorar constantemente mis habilidades.</p>
            </div>
        </div>
    </section>
    <section id="experiencia" class="experience">
        <h2>Experiencia</h2>
        <p>Tengo experiencia en:</p>
        <ul>
            <li>Desarrollo Frontend (HTML, CSS, JavaScript)</li>
            <li>Desarrollo Backend (Python )</li>
            <li>Bases de Datos (SQL, MongoDB)</li>
            <li>Frameworks y Librerías (React, Vue.js)</li>
            <!-- Agregar más según sea necesario -->
        </ul>
    </section>
    <section id="habilidades" class="skills">
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
    <section id="proyectos">
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
    <section id="contacto">
        <h2>Contacto</h2>
        <div class="social-icons">
            <a href="[https://www.instagram.com/](https://www.instagram.com/nico_tmrx_?igsh=MWs2eGtkNHZreHQ4ag%3D%3D&utm_source=qr)"><i class="fab fa-instagram"></i></a>
            <a href="https://www.linkedin.com/"><i class="fab fa-linkedin"></i></a>
            <a href="[https://wa.me](https://wa.me/3125534086"><i class="fab fa-whatsapp"></i></a>
            <a href="mailto:torresmolinanicolas838@gmail.com.com"><i class="fas fa-envelope"></i></a>
        </div>
    </section>
    <footer>
        &copy; 2024 Mi Portafolio
    </footer>
</body>
</html>
