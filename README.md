<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Minha Cartinha Para Você</title>
    <style>
        body {
            background-color: #e6e6fa; /* Roxo claro */
            font-family: Arial, sans-serif;
            text-align: center;
            color: #333;
            padding: 50px;
        }
        h1 {
            color: #6a0dad; /* Roxo mais escuro */
            font-size: 3em;
        }
        .envelope {
            width: 200px;
            height: 150px;
            background-color: #6a0dad; /* Envelope roxo */
            position: relative;
            display: inline-block;
            border-radius: 10px;
            margin-bottom: 20px;
        }
        .envelope:before {
            content: '';
            position: absolute;
            top: -20px;
            left: 0;
            right: 0;
            margin: auto;
            width: 0;
            height: 0;
            border-left: 100px solid transparent;
            border-right: 100px solid transparent;
            border-bottom: 20px solid #6a0dad;
        }
        .letter {
            display: none;
            margin-top: -150px;
            margin-left: auto;
            margin-right: auto;
            width: 180px;
            background-color: white; /* Cartinha branca */
            color: black; /* Texto preto */
            padding: 20px;
            border-radius: 10px;
            font-size: 1.2em;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            position: relative;
            z-index: 1;
        }
        .btn {
            margin-top: 30px;
            padding: 15px 30px;
            font-size: 1.2em;
            background-color: #6a0dad;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .btn:hover {
            background-color: #5a0ba8;
        }
    </style>
</head>
<body>
    <h1>Minha Cartinha Para Você</h1>
    <div class="envelope"></div>
    <button class="btn" onclick="showLetter()">Abrir Cartinha</button>
    <div class="letter" id="letter">
        <p>Você é minha paixão! 💖</p>
    </div>

    <script>
        function showLetter() {
            document.getElementById('letter').style.display = 'block';
        }
    </script>
</body>
</html>
