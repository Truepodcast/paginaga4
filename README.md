<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Página de Teste GA4</title>

  <!-- Google Analytics 4 -->
  <script async src="https://www.googletagmanager.com/gtag/js?id=G-980H5L7B0N"></script>
  <script>
    window.dataLayer = window.dataLayer || [];
    function gtag(){dataLayer.push(arguments);}
    gtag('js', new Date());
    gtag('config', 'G-980H5L7B0N');
  </script>
</head>
<body>
  <h1>Teste de coleta de dados GA4</h1>
  <p>Essa página está conectada ao Google Analytics 4.</p>
  <button id="btnEvento">Clique aqui</button>

  <script>
    document.getElementById('btnEvento').addEventListener('click', () => {
      gtag('event', 'botao_clicado', { descricao: 'Botão de teste clicado' });
      alert('Evento enviado para GA4!');
    });
  </script>
</body>
</html>
