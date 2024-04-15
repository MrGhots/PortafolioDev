
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi Portafolio</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #333;
            color: #fff;
            padding: 20px;
            text-align: center;
        }
        nav {
            display: flex;
            justify-content: center;
            background-color: #444;
            padding: 10px;
        }
        nav a {
            color: #fff;
            text-decoration: none;
            padding: 10px 20px;
        }
        section {
            padding: 20px;
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
            position: fixed;
            bottom: 0;
            width: 100%;
        }
    </style>
</head>
<body>
    <header>
        <h1>Mi Portafolio</h1>
    </header>
    <nav>
        <a href="#proyectos">Proyectos</a>
        <a href="#contacto">Contacto</a>
    </nav>
    <section id="proyectos">
        <h2>Proyectos</h2>
        <div class="projects">
            <div class="project">
                <img src="proyecto1.jpg" alt="Proyecto 1">
                <h3>Proyecto 1</h3>
                <p>Descripción del Proyecto 1</p>
            </div>
            <div class="project">
                <img src="proyecto2.jpg" alt="Proyecto 2">
                <h3>Proyecto 2</h3>
                <p>Descripción del Proyecto 2</p>
            </div>
            <!-- Agregar más proyectos según sea necesario -->
        </div>
    </section>
    <section id="contacto">
        <h2>Contacto</h2>
        <p>¡Ponte en contacto conmigo!</p>
        <form id="contactForm">
            <input type="text" placeholder="Nombre" required>
            <input type="email" placeholder="Correo electrónico" required>
            <textarea placeholder="Mensaje" required></textarea>
            <button type="submit">Enviar</button>
        </form>
    </section>
    <footer>
        &copy; 2024 Mi Portafolio
    </footer>
</body>
</html>
