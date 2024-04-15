<!DOCTYPE html>
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
        .contact-form {
            background-color: #fff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        .contact-form input[type="text"],
        .contact-form input[type="email"],
        .contact-form textarea {
            width: 100%;
            padding: 10px;
            margin-bottom: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
            box-sizing: border-box;
        }
        .contact-form textarea {
            height: 100px;
        }
        .contact-form button {
            background-color: #333;
            color: #fff;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }
        .contact-form button:hover {
            background-color: #555;
        }
        .contact-form p.success-message {
            color: green;
            font-weight: bold;
        }
        .contact-form p.error-message {
            color: red;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <header>
        <h1>Mi Portafolio</h1>
    </header>
    <nav>
        <a href="#sobre-mi">Sobre Mí</a>
        <a href="#experiencia">Experiencia</a>
        <a href="#habilidades">Habilidades</a>
        <a href="#proyectos">Proyectos</a>
        <a href="#contacto">Contacto</a>
    </nav>
    <section id="contacto">
        <h2>Contacto</h2>
        <p>¡Ponte en contacto conmigo!</p>
        <div class="contact-form">
            <?php
            if ($_SERVER["REQUEST_METHOD"] == "POST") {
                $nombre = $_POST['nombre'];
                $email = $_POST['email'];
                $mensaje = $_POST['mensaje'];

                $to = 'tudirecciondecorreo@example.com'; // Reemplaza con tu dirección de correo electrónico
                $subject = 'Mensaje de contacto desde Mi Portafolio';
                $message = "Nombre: $nombre\n";
                $message .= "Correo electrónico: $email\n";
                $message .= "Mensaje:\n$mensaje";

                $headers = "From: $email";

                if (mail($to, $subject, $message, $headers)) {
                    echo '<p class="success-message">¡Mensaje enviado con éxito!</p>';
                } else {
                    echo '<p class="error-message">¡Error al enviar el mensaje!</p>';
                }
            }
            ?>
            <form id="contactForm" method="post" action="<?php echo htmlspecialchars($_SERVER["PHP_SELF"]); ?>">
                <input type="text" name="nombre" placeholder="Nombre" required>
                <input type="email" name="email" placeholder="Correo electrónico" required>
                <textarea name="mensaje" placeholder="Mensaje" required></textarea>
                <button type="submit">Enviar</button>
            </form>
        </div>
    </section>
    <footer>
        &copy; 2024 Mi Portafolio
    </footer>
</body>
</html>
