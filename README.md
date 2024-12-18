<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Consolas Gamer</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #121212;
            color: white;
        }
        header {
            background-color: #1d1d1d;
            padding: 20px;
            text-align: center;
        }
        header h1 {
            font-size: 2.5em;
            margin: 0;
            color: #4CAF50; /* Verde */
        }
        nav {
            margin-top: 20px;
        }
        nav a {
            margin: 0 15px;
            text-decoration: none;
            color: #4CAF50; /* Verde */
            font-size: 1.1em;
        }
        nav a:hover {
            color: #ffffff;
        }
        .intro {
            background-image: url('https://files.oaiusercontent.com/file-WeM8ExddNbccXewhi5e5e2?se=2024-12-02T09%3A24%3A45Z&sp=r&sv=2024-08-04&sr=b&rscc=max-age%3D604800%2C%20immutable%2C%20private&rscd=attachment%3B%20filename%3D4e9c95c8-c7ec-4e1e-9469-e5e9a83d7caf.webp&sig=wrcm3qOeWOySwM/xTnevD5cmK7sJUFM%2BOdEFK44zR9Q%3D'); /* Cambiar imagen aquí */
            background-size: cover;
            background-position: center;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            color: white;
            position: relative;
        }
        .intro h2 {
            font-size: 3em;
            font-weight: bold;
            text-shadow: 2px 2px 10px rgba(0, 0, 0, 0.7);
        }
        .intro p {
            font-size: 1.3em;
            margin-top: 20px;
            text-shadow: 2px 2px 10px rgba(0, 0, 0, 0.5);
        }
        .button {
            margin-top: 30px;
            padding: 15px 30px;
            background-color: #4CAF50; /* Verde */
            color: white;
            font-size: 1.2em;
            text-decoration: none;
            border-radius: 5px;
            transition: background-color 0.3s;
        }
        .button:hover {
            background-color: #388E3C; /* Verde más oscuro */
        }
        .products {
            display: flex;
            justify-content: space-around;
            padding: 40px;
            background-color: #1c1c1c;
        }
        .product {
            text-align: center;
            margin: 0 20px;
            background-color: #333;
            padding: 20px;
            border-radius: 10px;
            width: 250px;
        }
        .product img {
            width: 100%;
            border-radius: 10px;
        }
        .product h3 {
            font-size: 1.5em;
            margin-top: 10px;
            color: #4CAF50; /* Verde */
        }
        .product p {
            font-size: 1.1em;
            color: #ddd;
        }
        footer {
            background-color: #1d1d1d;
            padding: 20px;
            text-align: center;
            color: #bbb;
            font-size: 0.9em;
        }
        .offer {
            background-color: #4CAF50; /* Verde */
            padding: 20px;
            color: white;
            text-align: center;
            border-radius: 10px;
            margin-top: 20px;
        }
        .offer h2 {
            font-size: 2em;
        }
    </style>
</head>
<body>

    <header>
        <h1>Consolas Gamer</h1>
        <nav>
            <a href="#inicio">Inicio</a>
            <a href="#consolas">Consolas</a>
            <a href="#ofertas">Ofertas</a>
        </nav>
    </header>

    <!-- Sección de Introducción -->
    <div class="intro" id="inicio">
        <div>
            <h2 style="
                font-size: 4em; 
                font-weight: bold; 
                color: #d1d409; 
                text-shadow: 3px 3px 10px rgba(0, 0, 0, 0.7), 0 0 20px #eeff00, 0 0 30px #fcf700;
                background: linear-gradient(90deg, #cffd03, #fdf902, #dbf301);
                -webkit-background-clip: text; 
                -webkit-text-fill-color: transparent;
            ">
                ¡Bienvenido a Consolas Gamer!
            </h2>
            <p style="
                font-size: 1.5em; 
                color: #FFFFFF; 
                text-shadow: 2px 2px 10px rgba(0, 0, 0, 0.5);
            ">
                Encuentra las mejores consolas y accesorios para tu experiencia gamer.
            </p>
            <a href="#consolas" class="button" id="jumpyButton" style="
                display: inline-block;
                padding: 15px 40px;
                font-size: 1.5em;
                font-weight: bold;
                color: #FFFFFF;
                text-decoration: none;
                border-radius: 50px;
                background: linear-gradient(135deg, #4CAF50, #00FF7F, #32CD32);
                box-shadow: 0 0 15px rgba(0, 255, 127, 0.7), 0 0 25px rgba(0, 255, 127, 0.5);
                animation: pulse-btn 2s infinite;
                transition: transform 0.2s ease, box-shadow 0.2s ease;
                position: relative;
            ">
                Explora nuestras consolas
            </a>
        </div>
    </div>
    
    <style>
        @keyframes pulse-btn {
            0% {
                box-shadow: 0 0 10px rgba(0, 255, 127, 0.7), 0 0 15px rgba(0, 255, 127, 0.5);
            }
            50% {
                box-shadow: 0 0 20px rgba(0, 255, 127, 1), 0 0 30px rgba(0, 255, 127, 0.8);
            }
            100% {
                box-shadow: 0 0 10px rgba(0, 255, 127, 0.7), 0 0 15px rgba(0, 255, 127, 0.5);
            }
        }
    </style>
    
    <script>
        const button = document.getElementById('jumpyButton');
    
        button.addEventListener('mouseover', () => {
            // Generar nuevas posiciones aleatorias dentro de la ventana
            const newX = Math.random() * (window.innerWidth - button.offsetWidth);
            const newY = Math.random() * (window.innerHeight - button.offsetHeight);
            
            // Aplicar las nuevas posiciones al botón
            button.style.position = 'absolute';
            button.style.left = `${newX}px`;
            button.style.top = `${newY}px`;
        });
    </script>
    
    

    <!-- Sección de Consolas -->
    <section class="products" id="consolas">
        <div class="product">
            <img src="https://i.blogs.es/15cd4e/captura_de_pantalla_2024-09-10_a_las_17.08.51/500_333.jpeg" alt="PS5">
            <h3>PlayStation 5</h3>
            <p>$499.99</p>
            <a href="#" class="button">Comprar</a>
        </div>
        <div class="product">
            <img src="https://m.media-amazon.com/images/I/61nq7mC0tHL.jpg" alt="Xbox Series X">
            <h3>Xbox Series X</h3>
            <p>$499.99</p>
            <a href="#" class="button">Comprar</a>
        </div>
        <div class="product">
            <img src="https://assets.mmsrg.com/isr/166325/c1/-/ASSET_MMS_85591077?x=536&y=402&format=jpg&quality=80&sp=yes&strip=yes&trim&ex=536&ey=402&align=center&resizesource&unsharp=1.5x1+0.7+0.02&cox=0&coy=0&cdx=536&cdy=402" alt="Nintendo Switch">
            <h3>Nintendo Switch</h3>
            <p>$299.99</p>
            <a href="#" class="button">Comprar</a>
        </div>
    </section>

    <!-- Sección de Ofertas -->
    <section class="offer" id="oferta-ps5">
        <h2>¡Oferta Especial!</h2>
        <p>¡Llévate la Play 5 con un mando y un juego a elegir!</p>
        <div class="product">
            <img src="https://i.blogs.es/aaf3fc/apertura-pack-playstation-5/450_1000.jpeg" alt="PS5 Oferta">
            <h3>PlayStation 5</h3>
            <p><strong>$449.99</strong> <del>$499.99</del></p>
            <a href="#" class="button">Comprar ahora</a>
        </div>
    </section>

    <!-- Sección de Segunda Oferta -->
    <section class="offer" id="oferta-xbox">
        <h2>¡Otra Oferta Especial!</h2>
        <p>¡Llévate una Xbox Serie X con un mando y un juego a elegir!</p>
        <div class="product">
            <img src="https://i.blogs.es/e0b594/apertura-pack-xbox-series-x-forza-horizon-5-ea-sports-fc-24/500_333.jpeg" alt="Xbox Oferta">
            <h3>Xbox Serie X</h3>
            <p><strong>$399.99</strong> <del>$499.99</del></p>
            <a href="#" class="button">Comprar ahora</a>
        </div>
    </section>

    <!-- Sección de Footer -->
    <footer id="contacto">
        <p>&copy; 2024 Consolas Gamer - Todos los derechos reservados</p>
    </footer>

</body>
</html>
