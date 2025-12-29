# Theusweb
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8" />
  <title>SecureStart | Segurança da Informação do Zero</title>
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <meta name="description" content="Guias práticos e acessíveis para aprender Segurança da Informação desde o básico. Planos a partir de R$29/mês." />
  <link rel="stylesheet" href="style.css">
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
</head>
<body>

  <!-- Skip link para acessibilidade -->
  <a class="skip-link" href="#main">Ir para o conteúdo</a>

  <header class="hero" role="banner">
    <div class="container">
      <h1>Aprenda Segurança da Informação do Zero</h1>
      <p>Guias práticos, simples e acessíveis para se proteger no mundo digital.</p>
      <a href="#planos" class="btn" role="button">Começar agora</a>
    </div>
  </header>

  <main id="main" class="site-main" role="main">
    <section class="section" aria-labelledby="o-que-aprender">
      <div class="container">
        <h2 id="o-que-aprender">O que você vai aprender</h2>
        <ul class="cards" aria-label="Principais tópicos">
          <li>🔐 Senhas seguras</li>
          <li>🎣 Como evitar golpes e phishing</li>
          <li>📶 Segurança em Wi‑Fi</li>
          <li>📜 LGPD para iniciantes</li>
          <li>🏪 Segurança para pequenos negócios</li>
        </ul>
      </div>
    </section>

    <section id="planos" class="section dark" aria-labelledby="planos-title">
      <div class="container">
        <h2 id="planos-title">Planos</h2>

        <div class="pricing" role="list">
          <article class="price-card" role="listitem" aria-label="Plano Básico">
            <h3>Básico</h3>
            <p class="price">R$ 29/mês</p>
            <p class="price-desc">Conteúdo essencial para começar.</p>
            <a class="btn" href="#" role="button" aria-label="Assinar plano Básico">Assinar</a>
          </article>

          <article class="price-card highlight" role="listitem" aria-label="Plano Pro">
            <h3>Pro</h3>
            <p class="price">R$ 59/mês</p>
            <p class="price-desc">Aulas extras, materiais e suporte.</p>
            <a class="btn" href="#" role="button" aria-label="Assinar plano Pro">Assinar</a>
          </article>

          <article class="price-card" role="listitem" aria-label="Plano Premium">
            <h3>Premium</h3>
            <p class="price">R$ 99/mês</p>
            <p class="price-desc">Acesso completo e consultoria.</p>
            <a class="btn" href="#" role="button" aria-label="Assinar plano Premium">Assinar</a>
          </article>
        </div>
      </div>
    </section>
  </main>

  <footer role="contentinfo">
    <div class="container">
      <p>© SecureStart - Educação em Segurança da Informação</p>
    </div>
  </footer>

</body>
</html>

/* Fonte e reset básico */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Inter', sans-serif;
}

:root{
  --bg: #0F172A;
  --panel: #020617;
  --muted: #E5E7EB;
  --accent: #2563EB;
  --accent-2: #22C55E;
  --card-border: rgba(255,255,255,0.06);
  --radius: 12px;
}

/* Skip link */
.skip-link {
  position: absolute;
  left: -9999px;
  top: auto;
  width: 1px;
  height: 1px;
  overflow: hidden;
}
.skip-link:focus {
  left: 1rem;
  top: 1rem;
  width: auto;
  height: auto;
  padding: 8px 12px;
  background: var(--accent);
  color: white;
  border-radius: 6px;
  z-index: 1000;
}

/* Base */
body {
  background: var(--bg);
  color: var(--muted);
  -webkit-font-smoothing:antialiased;
  -moz-osx-font-smoothing:grayscale;
  line-height: 1.5;
}

/* Layout helpers */
.container {
  max-width: 1100px;
  margin: 0 auto;
  padding: 0 20px;
}

/* Hero */
.hero {
  text-align: center;
  padding: 80px 20px;
}
.hero h1 {
  font-size: 2.25rem;
  margin-bottom: 16px;
  color: #fff;
}
.hero p {
  font-size: 1.05rem;
  margin-bottom: 24px;
  color: #cbd5e1;
}

/* Buttons */
.btn {
  display: inline-block;
  background: var(--accent);
  color: #fff;
  padding: 12px 22px;
  border-radius: 10px;
  text-decoration: none;
  font-weight: 600;
  transition: transform .12s ease, box-shadow .12s ease;
  box-shadow: 0 6px 18px rgba(37,99,235,0.12);
}
.btn:hover,
.btn:focus {
  transform: translateY(-2px);
  box-shadow: 0 10px 24px rgba(37,99,235,0.14);
}
.btn:focus {
  outline: 3px solid rgba(37,99,235,0.22);
  outline-offset: 3px;
}

/* Sections */
.section {
  padding: 60px 20px;
  text-align: center;
}
.section.dark {
  background: var(--panel);
}

/* Cards list */
.cards {
  list-style: none;
  display: grid;
  gap: 12px;
  max-width: 600px;
  margin: 24px auto 0;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
}
.cards li {
  background: rgba(255,255,255,0.03);
  padding: 12px 16px;
  border-radius: 10px;
  text-align: left;
  font-size: 1rem;
  display: flex;
  align-items: center;
  gap: 10px;
}

/* Pricing */
.pricing {
  display: grid;
  gap: 20px;
  max-width: 900px;
  margin: 20px auto 0;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
}

.price-card {
  background: rgba(255,255,255,0.02);
  padding: 24px;
  border-radius: var(--radius);
  border: 1px solid var(--card-border);
  text-align: center;
  display: flex;
  flex-direction: column;
  gap: 12px;
}
.price-card h3 {
  font-size: 1.15rem;
  color: #fff;
}
.price {
  font-size: 1.35rem;
  font-weight: 700;
  color: var(--accent);
}
.price-desc {
  color: #cbd5e1;
  font-size: 0.95rem;
}
.price-card .btn {
  margin-top: auto;
}

/* Highlighted card */
.price-card.highlight {
  border: 2px solid var(--accent-2);
  box-shadow: 0 8px 30px rgba(34,197,94,0.07);
}

/* Footer */
footer {
  text-align: center;
  padding: 30px 20px;
  color: #94a3b8;
}

/* Responsividade tipográfica */
@media (min-width: 900px) {
  .hero h1 { font-size: 3rem; }
  .hero p { font-size: 1.15rem; }
}

/* Respect user's reduced motion preference */
@media (prefers-reduced-motion: reduce) {
  .btn, .price-card {
    transition: none;
  }
}