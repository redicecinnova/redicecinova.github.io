<!DOCTYPE html>
<html lang="es, en, ch">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>REDICEC - Red de Innovación y Cooperación Académica Ecuador-China</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #ffffff;
            color: #333;
        }

        header {
            background-color: #0056b3;
            color: #fff;
            text-align: center;
            padding: 20px;
        }

        nav {
            background-color: #0073e6;
            padding: 10px;
        }

        nav ul {
            list-style: none;
            display: flex;
            justify-content: center;
            padding: 0;
            margin: 0;
        }

        nav ul li {
            margin: 0 15px;
        }

        nav ul li a {
            color: #fff;
            text-decoration: none;
            font-weight: bold;
        }

        .carousel {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 300px;
            background-color: #f0f0f0;
            position: relative;
        }

        .carousel img {
            max-height: 100%;
            max-width: 100%;
        }

        .carousel h2 {
            position: absolute;
            color: #fff;
            font-size: 24px;
            background-color: rgba(0, 0, 0, 0.6);
            padding: 10px 20px;
            border-radius: 5px;
        }

        .section {
            padding: 20px;
        }

        .section h2 {
            text-align: center;
            color: #0056b3;
        }

        .members {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
            text-align: center;
        }

        .members img {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            margin-bottom: 10px;
        }

        .contact-form {
            max-width: 600px;
            margin: auto;
            background-color: #f0f0f0;
            padding: 20px;
            border-radius: 5px;
        }

        footer {
            background-color: #0056b3;
            color: #fff;
            text-align: center;
            padding: 10px;
            margin-top: 20px;
        }
    </style>
</head>
<body>

<header>
    <h1>Bienvenidos a REDICEC</h1>
</header>

<nav>
    <ul>
        <li><a href="#intro">Introducción</a></li>
        <li><a href="#members">Miembros</a></li>
        <li><a href="#events">Eventos</a></li>
        <li><a href="#contact">Contacto</a></li>
    </ul>
</nav>

<div class="carousel">
    <h2>Conectando Ecuador y China a través de la Innovación</h2>
</div>

<section id="intro" class="section">
    <h2>Introducción</h2>
    <p>Red de Innovación y Cooperación Académica Ecuador-China. Después de varios encuentros académicos, surgió la idea de crear una Red de Científicos Ecuador-China. Formalizada el 24 de enero de 2024 en la Embajada de Ecuador en China y consolidada oficialmente el 27 de agosto del mismo año.</p>
    <p>REDICEC fomenta el intercambio de conocimientos y la investigación conjunta, conectando a investigadores y académicos de ambos países para desarrollar proyectos innovadores.</p>
</section>

<section id="members" class="section">
    <h2>Miembros</h2>
    <div class="members">
        <div>
            <img src="https://via.placeholder.com/100" alt="Miembro 1">
            <p>Nombre 1</p>
            <p>Posición</p>
        </div>
        <div>
            <img src="https://via.placeholder.com/100" alt="Miembro 2">
            <p>Nombre 2</p>
            <p>Posición</p>
        </div>
    </div>
</section>

<section id="events" class="section">
    <h2>Eventos</h2>
    <p>No te pierdas nuestro próximo simposio en diciembre de 2024: "Desarrollo Energético Sostenible: Desafíos y Oportunidades para Ecuador y China". ¡Regístrate aquí!</p>
</section>

<section id="contact" class="section">
    <h2>Contacto</h2>
    <div class="contact-form">
        <form>
            <label for="name">Nombre:</label><br>
            <input type="text" id="name" name="name" required><br><br>

            <label for="email">Correo:</label><br>
            <input type="email" id="email" name="email" required><br><br>

            <label for="message">Mensaje:</label><br>
            <textarea id="message" name="message" rows="4" required></textarea><br><br>

            <button type="submit">Enviar</button>
        </form>
    </div>
</section>

<footer>
    <p>REDICEC - © 2024</p>
</footer>

</body>
</html>
