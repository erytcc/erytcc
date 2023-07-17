**<!DOCTYPE html>
<html>
<head>
  <title>Super Mario - Busca de Peças</title>
  <style>
    #search-input {
      margin-bottom: 10px;
    }

    #search-results {
      display: none;
      margin-top: 10px;
    }

    .result {
      margin-bottom: 5px;
    }
  </style>
</head>
<body>
  <h1>Super Mario - Busca de Peças</h1>

  <div id="search">
    <input type="text" id="search-input" placeholder="Digite o código da peça">
    <button onclick="search()">Buscar</button>
  </div>

  <div id="search-results">
    <div class="result">
      <h3>Peça Encontrada</h3>
      <p>Nome da Peça: Nome da Peça</p>
      <p>Descrição: Descrição da Peça</p>
      <p>Onde Comprar: Local de Compra</p>
    </div>
  </div>

  <script>
    function search() {
      var input = document.getElementById("search-input").value;

      // Aqui você pode adicionar a lógica de pesquisa e obter as informações da peça com base no código fornecido.
      // Por exemplo, você pode consultar um banco de dados ou uma API para buscar as informações reais.

      // Neste exemplo, vamos apenas exibir informações de exemplo para ilustrar o funcionamento.
      var piece = {
        name: "Nome da Peça",
        description: "Descrição da Peça",
        whereToBuy: "Local de Compra"
      };

      // Atualiza a exibição dos resultados
      var resultsDiv = document.getElementById("search-results");
      var resultHtml = "<div class='result'>" +
                       "<h3>Peça Encontrada</h3>" +
                       "<p>Nome da Peça: " + piece.name + "</p>" +
                       "<p>Descrição: " + piece.description + "</p>" +
                       "<p>Onde Comprar: " + piece.whereToBuy + "</p>" +
                       "</div>";
      resultsDiv.innerHTML = resultHtml;
      resultsDiv.style.display = "block";
    }
  </script>
</body>
</html>
**
