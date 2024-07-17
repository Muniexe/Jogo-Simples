# Quadrado
Jogo Feito No GameMaker

<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Jogo Simples</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
    }
    h1 {
      color: #333;
    }
    button {
      padding: 10px 20px;
      font-size: 16px;
      margin: 10px;
      cursor: pointer;
      background-color: #4CAF50;
      color: white;
      border: none;
      border-radius: 4px;
      transition: background-color 0.3s;
    }
    button:hover {
      background-color: #45a049;
    }
  </style>
</head>
<body>
  <h1>Jogo Simples</h1>
  
  <p>Pressione o botão para jogar:</p>
  
  <button onclick="jogar()">Jogar</button>
  
  <p id="resultado"></p>
  
  <script>
    function jogar() {
      var numeroAleatorio = Math.floor(Math.random() * 10) + 1;
      var chute = prompt("Adivinhe o número de 1 a 10:");
      chute = parseInt(chute);
      
      if (chute === numeroAleatorio) {
        document.getElementById("resultado").innerHTML = "Parabéns! Você acertou!";
      } else {
        document.getElementById("resultado").innerHTML = "Que pena! O número correto era " + numeroAleatorio + ".";
      }
    }
  </script>
</body>
</html>
