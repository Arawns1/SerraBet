# SerraBet
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8">
    <title>Sistema de Apostas</title>
  </head>
  <body>
    <h1>Sistema de Apostas</h1>
    <p>Informe o valor da sua aposta:</p>
    <input type="number" id="aposta" name="aposta">
    <br>
    <button onclick="jogar()">Jogar</button>
    <br>
    <p id="resultado"></p>

    <script>
      function jogar() {
        var aposta = document.getElementById("aposta").value;
        var resultado = Math.floor(Math.random() * 2);
        if (resultado == 0) {
          document.getElementById("resultado").innerHTML = "Você perdeu a aposta de " + aposta + " reais.";
        } else {
          document.getElementById("resultado").innerHTML = "Você ganhou a aposta de " + aposta + " reais!";
        }
      }
    </script>
  </body>
</html>
https://S4nt1ag.github.io/SerraBet/
