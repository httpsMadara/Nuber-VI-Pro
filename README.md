# Nuber-VI-Pro
<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Vitor Carlos - Portfólio</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap');

  * {
    box-sizing: border-box;
  }
  body {
    margin: 0; padding: 0;
    background: #121212;
    color: #eee;
    font-family: 'Montserrat', sans-serif;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 100vh;
    text-align: center;
    padding: 1rem;
  }
  h1 {
    color: #00bcd4;
    font-weight: 700;
    margin-bottom: 0.5rem;
  }
  h2 {
    color: #ccc;
    margin-bottom: 1.5rem;
    font-weight: 400;
  }
  p {
    max-width: 600px;
    color: #bbb;
    line-height: 1.5;
  }
  .btn {
    margin-top: 2rem;
    background: #00bcd4;
    color: #121212;
    border: none;
    padding: 0.85rem 2rem;
    font-weight: 700;
    font-size: 1.1rem;
    border-radius: 30px;
    cursor: pointer;
    text-decoration: none;
    display: inline-block;
    transition: background 0.3s ease, transform 0.2s ease;
    box-shadow: 0 6px 12px rgba(0, 188, 212, 0.4);
  }
  .btn:hover,
  .btn:focus {
    background: #0097a7;
    transform: scale(1.05);
    box-shadow: 0 8px 16px rgba(0, 151, 167, 0.6);
  }
  footer {
    position: fixed;
    bottom: 10px;
    width: 100%;
    text-align: center;
    font-size: 0.85rem;
    color: #555;
  }
  @media (max-width: 480px) {
    h1 { font-size: 1.8rem; }
    h2 { font-size: 1.1rem; }
    p { font-size: 0.9rem; }
  }
</style>
</head>
<body>
  <h1>Vitor Carlos Santos</h1>
  <h2>Desenvolvedor em formação - Cruzeiro do Sul</h2>
  <p>Este projeto faz parte do meu portfólio de desenvolvimento. O <strong>Number VI Pro</strong> é um sistema de gestão de suporte técnico desenvolvido com foco em organização, praticidade e visual profissional.</p>
  <a href="dashboard.html" class="btn" aria-label="Acessar Dashboard">Acessar Dashboard</a>
  <footer>© 2025 Vitor Carlos Santos - Cruzeiro do Sul</footer>
</body>
</html>
<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Number VI Pro - Dashboard</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap');
  * {
    margin: 0; padding: 0; box-sizing: border-box;
    font-family: 'Montserrat', sans-serif;
  }
  body {
    background-color: #121212;
    color: #eee;
    display: flex;
    min-height: 100vh;
  }
  .sidebar {
    background-color: #1e1e1e;
    width: 220px;
    padding: 20px 15px;
    display: flex;
    flex-direction: column;
    box-shadow: 3px 0 8px rgba(0,0,0,0.7);
  }
  .sidebar h2 {
    color: #00bcd4;
    margin-bottom: 30px;
    font-weight: 700;
    font-size: 1.5rem;
  }
  .sidebar a {
    color: #ccc;
    text-decoration: none;
    margin: 12px 0;
    font-weight: 600;
    font-size: 1.05rem;
    padding: 8px 10px;
    border-radius: 8px;
    transition: background 0.25s ease, color 0.25s ease;
  }
  .sidebar a:hover,
  .sidebar a:focus {
    background-color: #00bcd4;
    color: #121212;
    outline: none;
    box-shadow: 0 0 8px #00bcd4;
    transform: translateX(4px);
  }
  .main {
    flex: 1;
    padding: 25px 30px;
    overflow-y: auto;
  }
  .card {
    background-color: #1f1f1f;
    border-radius: 12px;
    padding: 20px;
    margin-bottom: 20px;
    box-shadow: 0 4px 12px rgba(0, 188, 212, 0.3);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }
  .card:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 20px rgba(0, 188, 212, 0.6);
  }
  .card h3 {
    color: #00bcd4;
    margin-bottom: 10px;
    font-weight: 700;
    font-size: 1.4rem;
  }
  .card p {
    line-height: 1.5;
    color: #bbb;
  }
  .footer {
    position: fixed;
    bottom: 10px;
    left: 230px;
    color: #555;
    font-size: 12px;
  }
  /* Responsividade */
  @media (max-width: 768px) {
    body {
      flex-direction: column;
    }
    .sidebar {
      width: 100%;
      flex-direction: row;
      padding: 10px 20px;
      overflow-x: auto;
      box-shadow: 0 3px 8px rgba(0,0,0,0.7);
    }
    .sidebar h2 {
      margin-bottom: 0;
      margin-right: 30px;
      font-size: 1.2rem;
      white-space: nowrap;
      flex-shrink: 0;
    }
    .sidebar a {
      margin: 0 10px;
      padding: 10px 15px;
      white-space: nowrap;
    }
    .main {
      padding: 15px 20px;
      flex: none;
      height: auto;
    }
    .footer {
      position: static;
      margin-top: 10px;
      text-align: center;
      left: 0;
      width: 100%;
    }
  }
</style>
</head>
<body>
  <nav class="sidebar" aria-label="Menu lateral">
    <h2>Number VI Pro</h2>
    <a href="index.html" tabindex="0">Home</a>
    <a href="#" tabindex="0">Dashboard</a>
    <a href="#" tabindex="0">Tickets</a>
    <a href="#" tabindex="0">Chat</a>
    <a href="#" tabindex="0">Base de Conhecimento</a>
    <a href="#" tabindex="0">Relatórios</a>
    <a href="#" tabindex="0">Configurações</a>
  </nav>
  <main class="main" role="main">
    <section class="card" tabindex="0" aria-label="Resumo do Dashboard">
      <h3>Dashboard</h3>
      <p>Status de chamados, tickets em andamento e atividades recentes.</p>
    </section>
    <section class="card" tabindex="0" aria-label="Gerenciamento de Tickets">
      <h3>Gerenciamento de Tickets</h3>
      <p>Visualize, acompanhe e encerre chamados abertos.</p>
    </section>
    <section class="card" tabindex="0" aria-label="Base de Conhecimento">
      <h3>Base de Conhecimento</h3>
      <p>Busque soluções para problemas comuns de forma rápida e eficiente.</p>
    </section>
    <section class="card" tabindex="0" aria-label="Chat em Tempo Real">
      <h3>Chat em Tempo Real</h3>
      <p>Comunique-se diretamente com os técnicos para resolver chamados.</p>
    </section>
  </main>
  <footer class="footer" aria-label="Rodapé">
    Desenvolvido por Vitor Carlos Santos - Cruzeiro do Sul
  </footer>
</body>
</html>
``

