**<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SITE PERSONALIZAVEL</title>
    <style>
        body {
            font-family: var(--main-font, Arial), sans-serif;
            background-color: var(--background-color, white);
        }
        h1, h2, h3, h4 {
            color: var(--main-color, black);
        }
        .color-picker, .background-picker, .font-picker {
            margin: 10px 0;
        }
        .color-button, .background-button, .font-button {
            padding: 10px;
            margin: 5px;
            cursor: pointer;
            border: none;
            border-radius: 5px;
            color: white;
        }
        .color-button { color: white; }
        .red { background-color: red; }
        .green { background-color: green; }
        .blue { background-color: blue; }
        .black { background-color: black; }
        .white { background-color: white; color: black; border: 1px solid black; }
        .yellow { background-color: yellow; color: black; }
        .gray { background-color: gray; }
        .font-button { color: black; background-color: lightgray; }
    </style>
</head>
<body>
    <h1>Esse site é totalmente personalizavel</h1>
    <h2>Aqui coloque um subtitulo - OPCIONAL</h2>
    <h3>AQUI VOCE COLOCARIA O CONTEUDO</h3>
    <h4>COLOQUE ALGO A MAIS</h4>

    <div class="color-picker">
        <h3>Trocar Cor da Fonte:</h3>
        <button class="color-button red" onclick="changeColor('red')">Vermelho</button>
        <button class="color-button green" onclick="changeColor('green')">Verde</button>
        <button class="color-button blue" onclick="changeColor('blue')">Azul</button>
        <button class="color-button black" onclick="changeColor('black')">Preto</button>
        <button class="color-button white" onclick="changeColor('white')">Branco</button>
    </div>

    <div class="background-picker">
        <h3>Trocar Cor de Fundo:</h3>
        <button class="background-button red" onclick="changeBackgroundColor('red')">Vermelho</button>
        <button class="background-button green" onclick="changeBackgroundColor('green')">Verde</button>
        <button class="background-button blue" onclick="changeBackgroundColor('blue')">Azul</button>
        <button class="background-button black" onclick="changeBackgroundColor('black')">Preto</button>
        <button class="background-button white" onclick="changeBackgroundColor('white')">Branco</button>
        <button class="background-button yellow" onclick="changeBackgroundColor('yellow')">Amarelo</button>
        <button class="background-button gray" onclick="changeBackgroundColor('gray')">Cinza</button>
    </div>

    <div class="font-picker">
        <h3>Trocar Fonte:</h3>
        <button class="font-button" onclick="changeFont('Arial')">Arial</button>
        <button class="ont-button" onclick="changeFont('Georgia')">Georgia</button>
        <button class="font-button" onclick="changeFont('Times New Roman')">Times New Roman</button>
        <button class="font-button" onclick="changeFont('Courier New')">Courier New</button>
        <button class="ffont-button" onclick="changeFont('Verdana')">Verdana</button>
    </div>

    <script>
        function changeColor(color) {
            document.documentElement.style.setProperty('--main-color', color);
        }

        function changeBackgroundColor(color) {
            document.documentElement.style.setProperty('--background-color', color);
        }

        function changeFont(font) {
            document.documentElement.style.setProperty('--main-font', font);
        }
    </script>
</body>
</html>
**
