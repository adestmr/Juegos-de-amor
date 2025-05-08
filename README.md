<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Acertijos Mi Amor</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 0;
            padding: 20px;
            background-color: #f4f4f9;
        }
        .card {
            background-color: #fff;
            padding: 20px;
            margin: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        button {
            background-color: #ff6f61;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
        }
        button:hover {
            background-color: #e04d44;
        }
        h1 {
            color: #ff6f61;
        }
        .final {
            display: none;
        }
    </style>
</head>
<body>

    <h1>Bienvenido, Mi Amor</h1>

    <div class="card" id="acertijo1">
        <p>Acertijo 1: ¿Qué es lo que tiene un corazón pero no late?</p>
        <button onclick="mostrarCarta('acertijo2')">Resolver</button>
    </div>

    <div class="card" id="acertijo2" style="display:none;">
        <p>Acertijo 2: Si me nombras, dejo de existir. ¿Qué soy?</p>
        <button onclick="mostrarCarta('acertijo3')">Resolver</button>
    </div>

    <div class="card" id="acertijo3" style="display:none;">
        <p>Acertijo 3: Cuanto más quitas, más grande se vuelve. ¿Qué es?</p>
        <button onclick="mostrarCarta('final')">Resolver</button>
    </div>

    <div class="card final" id="final">
        <p>Mi amor, si has resuelto todos los acertijos, ¿te gustaría celebrar tu cumpleaños conmigo?</p>
        <button onclick="celebrar()">¡Sí, claro!</button>
    </div>

    <script>
        function mostrarCarta(id) {
            document.querySelectorAll('.card').forEach(function(card) {
                card.style.display = 'none';
            });
            document.getElementById(id).style.display = 'block';
        }

        function celebrar() {
            alert('¡Qué emoción! Te espero para celebrarlo. ❤️');
        }
    </script>

</body>
</html>
