<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi Página Web</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Bienvenido a Mi Página Web</h1>
        <nav>
            <ul>
                <li><a href="#">Inicio</a></li>
                <li><a href="#">Acerca de</a></li>
                <li><a href="#">Contacto</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section id="intro">
            <h2>Introducción</h2>
            <p>Esta es una página web de ejemplo creada con HTML5, CSS y JavaScript.</p>
            <button onclick="mostrarMensaje()">Haz clic aquí</button>
            <p id="mensaje" style="display:none;">¡Hola! Gracias por visitar mi página.</p>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 Mi Página Web. Todos los derechos reservados.</p>
    </footer>
    <script src="script.js"></script>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f0f0f0;
}

header {
    background-color: #333;
    color: white;
    padding: 1em 0;
    text-align: center;
}

nav ul {
    list-style: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin: 0 15px;
}

nav ul li a {
    color: white;
    text-decoration: none;
}

main {
    padding: 20px;
}

button {
    background-color: #333;
    color: white;
    border: none;
    padding: 10px 20px;
    cursor: pointer;
}

button:hover {
    background-color: #555;
}

footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 10px 0;
    position: fixed;
    width: 100%;
    bottom: 0;
}
function mostrarMensaje() {
    var mensaje = document.getElementById("mensaje");
    if (mensaje.style.display === "none") {
        mensaje.style.display = "block";
    } else {
        mensaje.style.display = "none";
    }
}




