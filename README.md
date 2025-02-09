<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¿Quieres ser mi San Valentín?</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            background-color: #fce4ec;
        }
        h1 {
            color: #d81b60;
        }
        p {
            font-size: 18px;
        }
        .buttons {
            margin-top: 20px;
        }
        button {
            font-size: 20px;
            padding: 10px 20px;
            margin: 10px;
            border: none;
            cursor: pointer;
        }
        #yes {
            background-color: #4CAF50;
            color: white;
        }
        #no {
            background-color: #f44336;
            color: white;
            position: absolute;
        }
        .dino {
            width: 150px;
            position: absolute;
        }
        .dino1 {
            top: 10%;
            left: 10%;
        }
        .dino2 {
            top: 10%;
            right: 10%;
        }
        .dino3 {
            bottom: 10%;
            left: 15%;
        }
        .dino4 {
            bottom: 10%;
            right: 15%;
        }
    </style>
</head>
<body>

    <h1>Fer, ¿quieres ser mi San Valentín?</h1>
    <p>Te amo, gracias por compartir tus días conmigo, eres el amor de mi vida.</p>

    <div class="buttons">
        <button id="yes" onclick="yesClicked()">Sí</button>
        <button id="no" onmouseover="moveNoButton()">No</button>
    </div>

    <!-- Dinosaurios decorativos -->
    <img src="https://i.imgur.com/5z8XzF8.png" class="dino dino1">
    <img src="https://i.imgur.com/5z8XzF8.png" class="dino dino2">
    <img src="https://i.imgur.com/5z8XzF8.png" class="dino dino3">
    <img src="https://i.imgur.com/5z8XzF8.png" class="dino dino4">

    <script>
        function yesClicked() {
            alert("¡Sabía que dirías que sí! Te amo 💖");
        }

        function moveNoButton() {
            let button = document.getElementById("no");
            let x = Math.random() * (window.innerWidth - 100);
            let y = Math.random() * (window.innerHeight - 50);
            button.style.left = `${x}px`;
            button.style.top = `${y}px`;
        }
    </script>

</body>
</html>
