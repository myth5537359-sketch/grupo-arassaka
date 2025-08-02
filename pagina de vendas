<html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Grupo Arassaka – Página de Vendas</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://unpkg.com/aos@next/dist/aos.css" />
  <style>
    body {
      margin: 0;
      font-family: 'Montserrat', sans-serif;
      background-color: #0d0d0d;
      color: #fff;
      scroll-behavior: smooth;
    }

    header {
      background: linear-gradient(to right, #0a0a0a, #1a1a1a);
      padding: 80px 20px;
      text-align: center;
    }

    .typewriter {
      font-size: 2.2rem;
      font-weight: 700;
      color: #00ccff;
      white-space: nowrap;
      overflow: hidden;
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 0 10px;
      font-family: 'Courier New', monospace;
    }

    .cursor {
      display: inline-block;
      background-color: #00ccff;
      width: 2px;
      height: 2rem;
      margin-left: 6px;
      animation: blink 0.7s infinite;
    }

    @keyframes blink {
      0%, 100% { opacity: 1; }
      50% { opacity: 0; }
    }

    header p {
      font-size: 1.2rem;
      color: #ccc;
      margin: 20px 0;
    }

    .cta-button {
      background-color: #00aaff;
      color: white;
      padding: 16px 32px;
      font-size: 1rem;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      transition: 0.3s;
    }

    .cta-button:hover {
      background-color: #0077cc;
    }

    .section {
      padding: 80px 20px;
      max-width: 1200px;
      margin: auto;
    }

    .section h2 {
      font-size: 2rem;
      margin-bottom: 20px;
      color: #00aaff;
    }

    .cards-container {
      display: flex;
      gap: 20px;
      overflow-x: auto;
      padding-bottom: 20px;
    }

    .card {
      background-color: #1a1a1a;
      flex: 0 0 280px;
      border-radius: 12px;
      padding: 20px;
      text-align: center;
    }

    .card h3 {
      color: #fff;
      margin-bottom: 10px;
    }

    .card p {
      font-size: 0.9rem;
      color: #aaa;
    }

    .card button {
      margin-top: 15px;
      background: #00aaff;
      color: #fff;
      border: none;
      padding: 10px 20px;
      border-radius: 6px;
      cursor: pointer;
    }

    .urgency {
      background-color: #1f1f1f;
      text-align: center;
      padding: 60px 20px;
    }

    .urgency h2 {
      color: #ff3333;
      font-size: 2rem;
    }

    .urgency p {
      font-size: 1.1rem;
      color: #ccc;
    }

    .founders {
      display: flex;
      flex-wrap: wrap;
      gap: 40px;
      align-items: center;
    }

    .founders img {
      width: 300px;
      border-radius: 12px;
    }

    .founders-text {
      flex: 1;
    }

    .benefits ul {
      list-style: none;
      padding: 0;
    }

    .benefits li {
      margin-bottom: 16px;
      display: flex;
      align-items: center;
    }

    .benefits li::before {
      content: "✔️";
      margin-right: 10px;
      color: #00aaff;
    }

    .testimonials {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
    }

    .testimonial {
      background-color: #1a1a1a;
      padding: 20px;
      border-radius: 10px;
      flex: 1 1 280px;
    }

    .faq-item {
      margin-bottom: 20px;
    }

    .faq-item h4 {
      color: #00aaff;
      margin-bottom: 5px;
    }

    .cta-final {
      background-color: #003366;
      text-align: center;
      padding: 60px 20px;
    }

    .cta-final h2 {
      font-size: 2rem;
      margin-bottom: 20px;
      color: #00ccff;
    }

    .footer {
      text-align: center;
      padding: 30px;
      background-color: #111;
      color: #555;
    }

    @media (max-width: 768px) {
      .founders {
        flex-direction: column;
        text-align: center;
      }

      .founders img {
        width: 100%;
      }
    }
  </style>
</head>
<body>
<!-- OFERTA POR TEMPO LIMITADO -->
<style>
.urgency {
  background: linear-gradient(135deg, #111 0%, #1a1a1a 100%);
  text-align: center;
  padding: 60px 20px;
  border-top: 2px solid #00ccff22;
  border-bottom: 2px solid #00ccff22;
  position: relative;
  overflow: hidden;
}

.urgency h2 {
  color: #ff4444;
  font-size: 2rem;
  margin-bottom: 10px;
}

.urgency p {
  font-size: 1.1rem;
  color: #ccc;
  margin-bottom: 20px;
}

#countdown {
  font-size: 1.8rem;
  font-weight: 700;
  color: #00ccff;
  animation: pulse 2s infinite;
}

@keyframes pulse {
  0% { opacity: 1; }
  50% { opacity: 0.6; }
  100% { opacity: 1; }
}
</style>

<section class="urgency" data-aos="zoom-in">
  <h2>⚠️ Oferta por tempo limitado!</h2>
  <p>Acesso vitalício. Últimos dias com esse valor promocional.</p>
  <div id="countdown">⏳ 48h restantes</div>
</section>

<script>
  const OFFER_DURATION_HOURS = 48;
  const STORAGE_KEY = "arassaka_offer_deadline";

  function getOrCreateDeadline() {
    const stored = localStorage.getItem(STORAGE_KEY);
    if (stored) return new Date(stored);

    const deadline = new Date();
    deadline.setHours(deadline.getHours() + OFFER_DURATION_HOURS);
    localStorage.setItem(STORAGE_KEY, deadline.toISOString());
    return deadline;
  }

  const offerDeadline = getOrCreateDeadline();

  function updateCountdown() {
    const now = new Date().getTime();
    const distance = offerDeadline - now;
    const countdownElement = document.getElementById("countdown");

    if (!countdownElement) return;

    if (distance <= 0) {
      countdownElement.innerHTML = "❌ Oferta encerrada!";
      countdownElement.style.color = "#ff4444";
      countdownElement.style.animation = "none";
      return;
    }

    const hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
    const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
    const seconds = Math.floor((distance % (1000 * 60)) / 1000);

    countdownElement.innerHTML = `⏳ ${hours}h ${minutes}m ${seconds}s restantes`;
  }

  setInterval(updateCountdown, 1000);
  updateCountdown();
</script>


  <!-- HERO MODERNO E IMPACTANTE -->
<style>
.hero {
  background: linear-gradient(to bottom, c#cc 60%, #111);
  padding: 80px 20px 40px;
  text-align: center;
  position: relative;
  overflow: hidden;
}

.hero h1 {
  font-size: 2.5rem;
  font-weight: 700;
  color: #00ccff;
  margin-bottom: 20px;
}

.hero p {
  font-size: 1.2rem;
  color: #ccc;
  max-width: 600px;
  margin: 0 auto 30px;
}

.hero-mockup {
  max-width: 400px;
  margin: 20px auto;
  border-radius: 12px;
  box-shadow: 0 0 20px #00ccff55;
  transition: 0.3s;
}

.hero .cta-button {
  padding: 16px 40px;
  font-size: 1.1rem;
  font-weight: 600;
  background-color: #00ccff;
  border: none;
  border-radius: 8px;
  color: #000;
  cursor: pointer;
  transition: background 0.3s;
}

.hero .cta-button:hover {
  background-color: #0d0d0d;
}
</style>

<section class="hero" data-aos="fade-in">
  <h1>Transforme sua Rotina. Domine seu Tempo.</h1>
  <p>Acesse agora os e-books do Grupo Arassaka e aprenda a usar o tempo como seu maior ativo.</p>
  
  <br>
  <button class="cta-button">Quero Acessar os Materiais</button>
</section>


  
  <!-- PRODUTOS -->
  <section class="section" data-aos="fade-up">
    <h2>Escolha seu Caminho</h2>
    <div class="cards-container">

      <div class="card">
        <img src="https://i.imgur.com/KuWVxUS.jpeg" alt="E-book O Valor do Tempo" style="width:100%; border-radius: 10px; margin-bottom: 15px;">
        <h3>O Valor do Tempo</h3>
        <p>E-book completo sobre gestão e consciência do tempo.</p>
        <p><strong style="color:#00ccff;font-size: 2.1rem;">R$ 39,90</strong></p>
        <button>COMPRE AGORA</button>
      </div>

      <div class="card">
        <img src="https://i.imgur.com/OodtfG4.jpeg" alt="E-book Método Seidō" style="width:100%; border-radius: 10px; margin-bottom: 15px;">
        <h3>Método Seidō</h3>
        <p>Disciplina e clareza mental em formato simbólico.</p>
        <p><strong style="color:#00ccff;font-size: 2.1rem;">R$ 39,90</strong></p>
        <button>COMPRE AGORA</button>
      </div>

      <div class="card" style="border: 2px solid #00ccff;">
        <img src="https://i.imgur.com/C4Rnak0.png" alt="Combo Arassaka" style="width:100%; border-radius: 10px; margin-bottom: 15px;">
        <h3>Combo Arassaka</h3>
        <p>Dois e-books por um preço promocional.</p>
        <p><strong style="color:#00ff99; font-size: 2.1rem;">R$ 64,90</strong></p>
        <button>COMPRE AGORA</button>
      </div>

    </div>
  </section>

  <!-- QUEM SOMOS -->
  <section class="section founders" data-aos="fade-right">
    <img src="fundadores.jpg" alt="Fundadores do Grupo Arassaka" />
    <div class="founders-text">
      <h2>Quem Somos</h2>
      <p>O Grupo Arassaka nasceu para redefinir como você enxerga o tempo. Unimos disciplina, estratégia e visão para ajudar pessoas comuns a conquistarem resultados extraordinários.</p>
    </div>
  </section>

 <!-- BENEFÍCIOS -->
<style>
.benefits-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 20px;
  margin-top: 30px;
}
.benefit-card {
  background-color: #1a1a1a;
  border: 1px solid #00aaff33;
  border-radius: 10px;
  padding: 20px;
  text-align: center;
  transition: all 0.3s ease;
}
.benefit-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 0 10px #00ccff55;
  border-color: #00ccff;
}
.benefit-card .icon {
  font-size: 2rem;
  color: #00ccff;
  display: block;
  margin-bottom: 10px;
}
.benefit-card p {
  font-size: 0.95rem;
  color: #ccc;
}
</style>

<section class="section benefits" data-aos="fade-up">
  <h2>Benefícios Reais</h2>
  <div class="benefits-grid">
    <div class="benefit-card" data-aos="fade-up" data-aos-delay="100">
      <span class="icon">⏱️</span>
      <p>Domine seu tempo com clareza</p>
    </div>
    <div class="benefit-card" data-aos="fade-up" data-aos-delay="200">
      <span class="icon">🎯</span>
      <p>Aumente seu foco e disciplina</p>
    </div>
    <div class="benefit-card" data-aos="fade-up" data-aos-delay="300">
      <span class="icon">🧠</span>
      <p>Planeje metas de forma prática</p>
    </div>
    <div class="benefit-card" data-aos="fade-up" data-aos-delay="400">
      <span class="icon">🌀</span>
      <p>Reduza ansiedade com organização</p>
    </div>
    <div class="benefit-card" data-aos="fade-up" data-aos-delay="500">
      <span class="icon">💡</span>
      <p>Visual minimalista e funcional</p>
    </div>
  </div>
</section>

  <!-- DEPOIMENTOS -->
  <section class="section" data-aos="zoom-in-up">
    <h2>Depoimentos Reais</h2>
    <div class="testimonials">
      <div class="testimonial">
        <p>"Nunca imaginei que um e-book mudaria minha rotina assim. Obrigado, Arassaka!"</p>
        <strong>– Lucas M.</strong>
      </div>
      <div class="testimonial">
        <p>"O Planner gratuito já me deu mais foco do que meses de terapia. Sério."</p>
        <strong>– Camila R.</strong>
      </div>
      <div class="testimonial">
        <p>"Comprei o combo e foi a melhor compra do ano. Visual incrível e direto ao ponto."</p>
        <strong>– Rafael S.</strong>
      </div>
    </div>
  </section>

  <!-- GARANTIA -->
  <section class="section" data-aos="fade-up">
    <h2>Garantia Total</h2>
    <p>✔️ Garantia incondicional de 7 dias. Seu risco é ZERO.</p>
  </section>

  <!-- FAQ -->
  <section class="section" data-aos="fade-in">
    <h2>Dúvidas Frequentes</h2>
    <div class="faq-item"><h4>Como recebo os materiais?</h4><p>Você recebe tudo por e-mail logo após a compra.</p></div>
    <div class="faq-item"><h4>Funciona em celular?</h4><p>Sim! Todos os arquivos são compatíveis com desktop e mobile.</p></div>
    <div class="faq-item"><h4>Por quanto tempo terei acesso?</h4><p>Acesso vitalício e ilimitado.</p></div>
    <div class="faq-item"><h4>Como funciona a garantia?</h4><p>Você pode pedir reembolso em até 7 dias após a compra.</p></div>
  </section>

  <!-- CTA FINAL -->
  <section class="cta-final" data-aos="zoom-in">
    <h2>Escolha transformar sua rotina agora</h2>
    <button class="cta-button">Acessar os materiais</button>
  </section>

  <footer class="footer">
    © 2025 Grupo Arassaka. Todos os direitos reservados.
  </footer>

  <!-- Scripts -->
  <script src="https://unpkg.com/aos@next/dist/aos.js"></script>
  <script>
    AOS.init();
  </script>

  <script>
    const text = "Transforme sua Rotina com o Grupo Arassaka";
    let index = 0;
    const speed = 60;

    function typeWriter() {
      if (index < text.length) {
        document.getElementById("typed-text").innerHTML += text.charAt(index);
        index++;
        setTimeout(typeWriter, speed);
      }
    }

    document.addEventListener("DOMContentLoaded", typeWriter);
  </script>
</body>
</html>
