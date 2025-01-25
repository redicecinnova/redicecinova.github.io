<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Página Mejorada</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        /* Paleta de colores */
        :root {
            --color-1: #54668E; /* Azul oscuro */
            --color-2: #879EC6; /* Azul claro */
            --color-3: #363955; /* Gris oscuro */
            --color-4: #F5F6E6; /* Crema */
            --color-5: #E8E8E8; /* Gris claro */
        }

        /* General */
        body {
            margin: 0;
            font-family: 'Poppins', sans-serif;
            scroll-behavior: smooth;
        }

        /* Encabezado */
        header {
            background-color: var(--color-1);
            color: var(--color-4);
            text-align: center;
            padding: 20px;
        }

        header img {
            max-width: 150px;
            height: auto;
            margin-bottom: 10px;
        }

        /* Navegación */
        nav {
            background-color: var(--color-3);
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
            color: var(--color-4);
            text-decoration: none;
            font-weight: bold;
        }

        nav ul li a:hover {
            text-decoration: underline;
        }

        nav ul li:first-child {
            margin-left: 0;
        }

        nav ul li:last-child {
            margin-right: 0;
        }

        /* Selector de idioma */
        .language-selector {
            position: absolute;
            top: 10px;
            right: 10px;
        }

        .language-selector button {
            background-color: var(--color-2);
            color: var(--color-4);
            border: none;
            padding: 5px 10px;
            cursor: pointer;
            border-radius: 5px;
            font-size: 14px;
        }

        .language-selector button:hover {
            background-color: var(--color-1);
        }

        /* Carrusel básico */
        .carousel {
            position: relative;
            width: 80%;
            margin: 20px auto;
            overflow: hidden;
            border: 2px solid var(--color-2);
            border-radius: 10px;
        }

        .carousel img {
            width: 100%;
            display: block;
        }

        /* Miembros */
        .section {
            padding: 20px;
            background-color: var(--color-5);
        }

        .section h2 {
            text-align: center;
            color: var(--color-1);
        }

        .carousel-buttons {
            position: absolute;
            top: 50%;
            width: 100%;
            display: flex;
            justify-content: space-between;
            transform: translateY(-50%);
        }

        .carousel-buttons button {
            background-color: var(--color-3);
            color: var(--color-4);
            border: none;
            padding: 10px;
            cursor: pointer;
            border-radius: 50%;
            box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.2);
            transition: transform 0.2s;
        }

        .carousel-buttons button:hover {
            background-color: var(--color-1);
            transform: scale(1.1);
        }

        /* Pie de página */
        footer {
            background-color: var(--color-1);
            color: var(--color-4);
            text-align: center;
            padding: 20px;
        }

        footer .social-links {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-top: 10px;
        }

        footer .social-links a {
            color: var(--color-4);
            text-decoration: none;
            font-size: 20px;
        }

        footer .social-links a:hover {
            color: var(--color-2);
        }

        footer .additional-links {
            margin-top: 15px;
            font-size: 14px;
        }

        footer .additional-links a {
            color: var(--color-4);
            text-decoration: none;
            margin: 0 10px;
        }

        footer .additional-links a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <div class="language-selector">
        <button onclick="translatePage('es')">ES</button>
        <button onclick="translatePage('en')">EN</button>
        <button onclick="translatePage('zh')">中文</button>
    </div>

    <header>
        <img src="logo.png" alt="Logo de la página">
        <h1 id="title">Bienvenidos a Nuestra Página</h1>
    </header>

    <nav>
        <ul>
            <li><a href="#introduccion" id="nav-intro">Introducción</a></li>
            <li><a href="#miembros" id="nav-miembros">Miembros</a></li>
            <li><a href="#eventos" id="nav-eventos">Eventos</a></li>
            <li><a href="#convocatoria" id="nav-convocatoria">Convocatoria</a></li>
        </ul>
    </nav>

    <section class="section" id="introduccion">
        <h2>Introducción</h2>
        <p>Bienvenidos a la sección de introducción. Aquí encontrarás información general sobre nuestra página.</p>
    </section>

    <section class="section" id="miembros">
        <h2 id="miembros-title">Miembros</h2>
        <div class="carousel">
            <img src="miembro1.jpg" alt="Miembro 1" loading="lazy">
            <img src="miembro2.jpg" alt="Miembro 2" loading="lazy">
            <img src="miembro3.jpg" alt="Miembro 3" loading="lazy">
            <div class="carousel-buttons">
                <button id="prev">&#10094;</button>
                <button id="next">&#10095;</button>
            </div>
        </div>
    </section>

    <section class="section" id="eventos">
        <h2>Eventos</h2>
        <p>Consulta los próximos eventos y actividades en nuestra comunidad.</p>
    </section>

    <section class="section" id="convocatoria">
        <h2 id="convocatoria-title">Convocatoria para Capítulos de Libro</h2>
        <p id="convocatoria-text" style="text-align: center; color: var(--color-1);">Próximamente más información sobre cómo participar en nuestra convocatoria de capítulos de libro.</p>
    </section>

    <footer>
        <p id="footer-text">&copy; 2025 Nuestra Página</p>
        <div class="social-links">
            <a href="https://www.linkedin.com/company/105199794/" target="_blank">LinkedIn</a>
            <a href="https://www.facebook.com/profile.php?id=61571781744764" target="_blank">Facebook</a>
            <a href="https://mp.weixin.qq.com/s/HfIHBz-G_aAo1YJzN7vR7g" target="_blank">WeChat</a>
            <a href="https://www.instagram.com/redicec1?igsh=MXdsY2xlbmk2Nmc3Mg==" target="_blank">Instagram</a>
        </div>
        <div class="additional-links">
            <a href="#">Política de privacidad</a>
            <a href="#">Términos y condiciones</a>
            <a href="#">Mapa del sitio</a>
        </div>
        <p>Email: <a href="mailto:redicec39@gmail.com">redicec39@gmail.com</a></p>
    </footer>

    <script>
        const translations = {
            es: {
                title: "Bienvenidos a Nuestra Página",
                "nav-intro": "Introducción",
                "nav-miembros": "Miembros",
                "nav-eventos": "Eventos",
                "nav-convocatoria": "Convocatoria",
                "miembros-title": "Miembros",
                "convocatoria-title": "Convocatoria para Capítulos de Libro",
                "convocatoria-text": "Próximamente más información sobre cómo participar en nuestra convocatoria de capítulos de libro.",
                "footer-text": "&copy; 2025 Nuestra Página",
            },
            en: {
                title: "Welcome to Our Page",
                "nav-intro": "Introduction",
                "nav-miembros": "Members",
                "nav-eventos": "Events",
                "nav-convocatoria": "Call for Chapters",
                "miembros-title": "Members",
                "convocatoria-title": "Call for Book Chapters",
                "convocatoria-text": "More information coming soon about how to participate in our call for book chapters.",
                "footer-text": "&copy; 2025 Our Page",
            },
            zh: {
                title: "欢迎访问我们的网站",
                "nav-intro": "介绍",
                "nav-miembros": "成员",
                "nav-eventos": "活动",
                "nav-convocatoria": "征集章节",
                "miembros-title": "成员",
                "convocatoria-title": "书籍章节征集",
                "convocatoria-text": "关于如何参与我们的书籍章节征集，更多信息即将发布。",
                "footer-text": "&copy; 2025 我们的页面",
            }
        };

        function translatePage(lang) {
            for (const [id, text] of Object.entries(translations[lang])) {
                const element = document.getElementById(id);
                if (element) {
                    element.innerHTML = text;
                }
            }
        }
    </script>
</body>
</html>
