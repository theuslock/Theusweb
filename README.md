# Theusweb
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <title>SecureStart | Segurança da Informação do Zero</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <link rel="stylesheet" href="style.css">
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
</head>
<body>

<header class="hero">
  <h1>Aprenda Segurança da Informação do Zero</h1>
  <p>Guias práticos, simples e acessíveis para se proteger no mundo digital.</p>
  <a href="#planos" class="btn">Começar agora</a>
</header>

<section class="section">
  <h2>O que você vai aprender</h2>
  <ul class="cards">
    <li>🔐 Senhas seguras</li>
    <li>🎣 Como evitar golpes e phishing</li>
    <li>📶 Segurança em Wi-Fi</li>
    <li>📜 LGPD para iniciantes</li>
    <li>🏪 Segurança para pequenos negócios</li>
  </ul>
</section>

<section id="planos" class="section dark">
  <h2>Planos</h2>
  <div class="pricing">
    <div class="price-card">
      <h3>Básico</h3>
      <p>R$ 29/mês</p>
      <a class="btn">Assinar</a>
    </div>
    <div class="price-card highlight">
      <h3>Pro</h3>
      <p>R$ 59/mês</p>
      <a class="btn">Assinar</a>
    </div>
    <div class="price-card">
      <h3>Premium</h3>
      <p>R$ 99/mês</p>
      <a class="btn">Assinar</a>
    </div>
  </div>
</section>

<footer>
  <p>© SecureStart - Educação em Segurança da Informação</p>
</footer>

</body>
</html>

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Inter', sans-serif;
}

body {
  background: #0F172A;
  color: #E5E7EB;
}

.hero {
  text-align: center;
  padding: 80px 20px;
}

.hero h1 {
  font-size: 2.5rem;
  margin-bottom: 20px;
}

.hero p {
  font-size: 1.2rem;
  margin-bottom: 30px;
}

.btn {
  background: #2563EB;
  color: #fff;
  padding: 14px 28px;
  border-radius: 8px;
  text-decoration: none;
  font-weight: 600;
}

.section {
  padding: 60px 20px;
  text-align: center;
}

.section.dark {
  background: #020617;
}

.cards {
  list-style: none;
  display: grid;
  gap: 15px;
  max-width: 600px;
  margin: auto;
}

.pricing {
  display: grid;
  gap: 20px;
  max-width: 900px;
  margin: auto;
}

.price-card {
  background: #020617;
  padding: 30px;
  border-radius: 12px;
}

.price-card.highlight {
  border: 2px solid #22C55E;
}

footer {
  text-align: center;
  padding: 30px;
  font-size: 0.9rem;
}