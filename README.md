# PROYECTO-DE-GRADO
(http://127.0.0.1:5500/Templates/index.html#mapa)

Còdigo de HTML:
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cambio Climático</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="styles.css"> <!-- Enlace al archivo CSS externo -->
    <style>
        body {
            font-family: 'Montserrat', sans-serif;
            margin: 0;
            padding: 0;
        }

        header {
            background-color: #2d6a4f; /* Verde oscuro */
            color: white;
            padding: 10px 20px;
            text-align: center;
        }

        nav {
            background-color: #2d6a4f; /* Verde oscuro */
            padding: 10px;
            text-align: center;
        }

        nav a {
            margin: 0 10px;
            color: white;
            text-decoration: none;
            font-weight: bold;
            cursor: pointer;
        }

        nav a:hover {
            text-decoration: underline;
        }

        section {
            display: none;
            padding: 20px;
        }

        section.active {
            display: block;
        }

        .hero {
            background-color: #d8f3dc;
            text-align: center;
            padding: 50px 20px;
        }

        .info-point {
            position: absolute;
            width: 15px;
            height: 15px;
            background-color: #ff6347;
            border-radius: 50%;
            cursor: pointer;
        }

        .info-popup {
            position: absolute;
            background-color: white;
            border: 1px solid #ccc;
            padding: 10px;
            display: none;
            width: 200px;
            box-shadow: 0px 0px 5px rgba(0, 0, 0, 0.2);
            z-index: 10;
        }

        #mapa-contenedor {
            position: relative;
            width: 100%;
            height: 500px;
            background: url('img/MAPA.jpg') no-repeat center/cover;
            margin: 20px 0;
        }

        footer {
            background-color: #2d6a4f; /* Verde oscuro */
            color: white;
            text-align: center;
            padding: 10px;
            margin-top: 20px;
        }

        footer p {
            font-size: 14px;
        }
    </style>
</head>
<body>
    <header>
        <h1>Cambio Climático 🌍</h1>
    </header>
    <nav>
        <a href="#inicio" onclick="mostrarSeccion('inicio')">Inicio 🏡</a>
        <a href="#widget" onclick="mostrarSeccion('widget')">Datos Curiosos 🧐</a>
        <a href="#consejos" onclick="mostrarSeccion('consejos')">Consejos 🌱</a>
        <a href="#tips" onclick="mostrarSeccion('tips')">Tips 💡</a>
        <a href="#informacion" onclick="mostrarSeccion('informacion')">Información 📚</a>
        <a href="#mapa" onclick="mostrarSeccion('mapa')">Mapa Interactivo 🗺️</a>
    </nav>
    <section class="hero active" id="inicio">
        <h1>Bienvenidos a la Página del Cambio Climático</h1>
        <p>Descubre cómo el cambio climático está afectando nuestro planeta y cómo podemos marcar la diferencia. 🌎🌱</p>
    </section>
    <section id="widget">
        <h2>Datos Curiosos sobre el Cambio Climático 🌡️</h2>
        <ul>
            <li>El año más cálido registrado fue 2016 🏆🌞.</li>
            <li>El Ártico se calienta casi tres veces más rápido que el resto del mundo 🐧❄️.</li>
            <li>Más del 90% del exceso de calor es absorbido por los océanos 🌊🔥.</li>
            <li>El cambio climático está provocando la desaparición de especies animales únicas 🦏🐆.</li>
        </ul>
    </section>
    <section id="consejos">
        <h2>Consejos para Evitar el Cambio Climático ♻️</h2>
        <ul>
            <li>Reduce el consumo de carne 🥩➡️🥗.</li>
            <li>Usa transporte público o camina 🚶‍♂️🚆.</li>
            <li>Planta árboles y cuida la naturaleza 🌳🌻.</li>
            <li>Apaga las luces cuando no las necesites 💡🚫.</li>
            <li>Reduce, reutiliza y recicla ♻️.</li>
        </ul>
    </section>
    <section id="tips">
        <h2>Tips para Luchar contra el Cambio Climático 🌿</h2>
        <ul>
            <li>Haz un consumo responsable de recursos 🌍💧.</li>
            <li>Apoya políticas ecológicas y energías renovables ⚡🌞.</li>
            <li>Usa menos plástico y promueve alternativas ecológicas 🛍️🌍.</li>
            <li>Participa en iniciativas de limpieza comunitaria 🧹🏘️.</li>
        </ul>
    </section>
    <section id="informacion">
        <h2>Información Extra 📖</h2>
        <h3>Anecdota Infantil 🧸</h3>
        <p>Un grupo de niños decidió plantar árboles y descubrió que juntos podían vencer al "monstruo invisible" del cambio climático. Cada árbol que plantaban representaba una victoria para el planeta 🌳💚.</p>
        <h3>Anecdota para Adultos 🌍</h3>
        <p>En un pueblo costero, los habitantes restauraron humedales y aprendieron a convivir con el cambio climático, convirtiéndose en un modelo para otros pueblos. Su ejemplo inspiró a muchas personas a tomar acción 👩‍🌾🌊.</p>
    </section>
    <section id="mapa">
        <h2>Mapa Interactivo del Cambio Climático 🗺️</h2>
        <p>Pasa el mouse sobre los puntos para obtener más información 📍.</p>
        <div id="mapa-contenedor">
            <div class="info-point" style="top: 50px; left: 100px;" data-info="El derretimiento del Ártico está afectando los ecosistemas polares. 🐻‍❄️❄️"></div>
            <div class="info-point" style="top: 200px; left: 300px;" data-info="El aumento del nivel del mar amenaza islas como las Maldivas 🏝️🌊."></div>
            <div class="info-point" style="top: 350px; left: 500px;" data-info="Las olas de calor extremo son cada vez más comunes 🥵🔥."></div>
        </div>
    </section>
    <footer>
        <p>&copy; 2025 @GabyGabsShow. Todos los derechos reservados. 💻🌍</p>
    </footer>
    <script>
        function mostrarSeccion(id) {
            document.querySelectorAll('section').forEach(section => {
                section.classList.remove('active');
            });
            document.getElementById(id).classList.add('active');
        }

        document.querySelectorAll('.info-point').forEach(point => {
            point.addEventListener('mouseenter', function () {
                const info = this.getAttribute('data-info');
                const popup = document.createElement('div');
                popup.className = 'info-popup';
                popup.innerText = info;
                document.body.appendChild(popup);

                const rect = this.getBoundingClientRect();
                popup.style.left = `${rect.left + window.scrollX + 20}px`;
                popup.style.top = `${rect.top + window.scrollY - 10}px`;
                popup.style.display = 'block';
            });

            point.addEventListener('mouseleave', function () {
                document.querySelectorAll('.info-popup').forEach(popup => popup.remove());
            });
        });
    </script>
</body>
</html>





Code de STYLE.CSS:
/* Estilos generales */
body {
    margin: 0;
    padding: 0;
    font-family: 'Montserrat', sans-serif; /* Asegura que se use Montserrat */
    background-color: #f4f9f9; /* Fondo suave */
    color: #2c3e50;
    line-height: 1.6;
}

/* Estilos del header */
header {
    background-color: #2d6a4f; /* Verde inspirado en la naturaleza */
    color: white;
    padding: 1.5rem 2rem;
    text-align: center;
    box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
    margin-bottom: 1rem;
}

header h1 {
    font-size: 2.5rem;
    margin: 0;
    letter-spacing: 2px;
}

/* Estilos del menú de navegación */
nav {
    display: flex;
    justify-content: center;
    gap: 1.5rem;
    background-color: #1b4332; /* Verde oscuro */
    padding: 1rem 0;
    box-shadow: 0 2px 6px rgba(0, 0, 0, 0.1);
}

nav a {
    color: white;
    text-decoration: none;
    font-weight: 600;
    font-size: 1.1rem;
    transition: color 0.3s ease;
    padding: 0.5rem 1rem;
}

nav a:hover {
    color: #74c69d; /* Verde claro */
    background-color: #2d6a4f;
    border-radius: 5px;
}

/* Sección hero */
.hero {
    text-align: center;
    padding: 3rem 2rem;
    background: linear-gradient(135deg, #74c69d, #52b788); /* Tonos del planeta */
    color: white;
}

.hero h1 {
    font-size: 2.5rem;
    margin: 0;
}

.hero p {
    font-size: 1.2rem;
    margin-top: 0.5rem;
}

/* Secciones generales */
section {
    padding: 2rem;
    margin-bottom: 2rem;
}

section h2 {
    font-size: 2rem;
    margin-bottom: 1rem;
}

section ul {
    list-style: none;
    padding-left: 0;
}

section ul li {
    font-size: 1.1rem;
    margin-bottom: 1rem;
}

/* Estilos para el mapa */
#mapa-contenedor {
    position: relative;
    width: 100%;
    height: 500px;
    background: url('img/MAPA.jpg') no-repeat center/cover;
    margin: 2rem 0;
}

/* Estilos del footer */
footer {
    background-color: #2d6a4f; /* Verde oscuro */
    color: white;
    text-align: center;
    padding: 1rem;
    margin-top: 2rem;
}

footer p {
    font-size: 1rem;
    margin: 0;
}

/* Estilo para las burbujas de información en el mapa */
.info-point {
    position: absolute;
    width: 15px;
    height: 15px;
    background-color: #ff6347;
    border-radius: 50%;
    cursor: pointer;
}

.info-popup {
    position: absolute;
    background-color: white;
    border: 1px solid #ccc;
    padding: 10px;
    display: none;
    width: 200px;
    box-shadow: 0px 0px 5px rgba(0, 0, 0, 0.2);
    z-index: 10;
}
