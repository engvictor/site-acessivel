
<!DOCTYPE html>
<html lang="pt-BR">

<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />

  <title>Site Acessível</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: Arial, sans-serif;
      background: #f4f7fb;
      color: #222;
      line-height: 1.7;
      transition: 0.3s ease;
      font-size: 16px;
    }

    header {
      background: #003366;
      color: white;
      text-align: center;
      padding: 40px 20px;
    }

    header h1 {
      font-size: 2.5rem;
      margin-bottom: 10px;
    }

    header p {
      max-width: 700px;
      margin: auto;
    }

    nav {
      background: white;
      display: flex;
      justify-content: center;
      gap: 15px;
      flex-wrap: wrap;
      padding: 15px;
      position: sticky;
      top: 0;
      z-index: 999;
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
    }

    nav a {
      text-decoration: none;
      color: #003366;
      font-weight: bold;
      padding: 10px 15px;
      border-radius: 10px;
      transition: 0.2s;
    }

    nav a:hover,
    nav a:focus {
      background: #dbe9ff;
      outline: none;
    }

    main {
      max-width: 1100px;
      margin: auto;
      padding: 30px 20px;
    }

    .section {
      background: white;
      padding: 25px;
      margin-bottom: 30px;
      border-radius: 18px;
      box-shadow: 0 2px 12px rgba(0,0,0,0.08);
    }

    .section h2 {
      color: #003366;
      margin-bottom: 15px;
    }

    .cards {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
      gap: 20px;
      margin-top: 20px;
    }

    .card {
      background: #eef5ff;
      padding: 20px;
      border-radius: 14px;
    }

    .card h3 {
      color: #003366;
      margin-bottom: 10px;
    }

    .controls {
      position: fixed;
      right: 15px;
      bottom: 15px;
      background: white;
      width: 260px;
      padding: 15px;
      border-radius: 18px;
      box-shadow: 0 0 15px rgba(0,0,0,0.2);
      z-index: 1000;
      display: flex;
      flex-direction: column;
      gap: 10px;
    }

    .controls-title {
      text-align: center;
      font-weight: bold;
      color: #003366;
      margin-bottom: 5px;
    }

    .buttons-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 10px;
    }

    button {
      border: none;
      background: #003366;
      color: white;
      padding: 12px;
      border-radius: 10px;
      cursor: pointer;
      font-weight: bold;
      transition: 0.2s;
      font-size: 0.9rem;
    }

    button:hover {
      background: #0052aa;
      transform: scale(1.03);
    }

    button:focus {
      outline: 3px solid #ffcc00;
    }

    .font-control {
      display: flex;
      flex-direction: column;
      gap: 5px;
    }

    .font-control label {
      font-weight: bold;
      font-size: 0.9rem;
    }

    .font-control input {
      width: 100%;
    }

    footer {
      background: #003366;
      color: white;
      text-align: center;
      padding: 25px;
      margin-top: 40px;
    }

    .color-red {
      color: red;
      font-weight: bold;
    }

    .color-green {
      color: green;
      font-weight: bold;
    }

    .color-blue {
      color: blue;
      font-weight: bold;
    }

    /* Alto contraste */

    .high-contrast {
      background: black;
      color: yellow;
    }

    .high-contrast header,
    .high-contrast nav,
    .high-contrast .section,
    .high-contrast .controls,
    .high-contrast footer {
      background: #111;
      color: yellow;
      border: 1px solid yellow;
    }

    .high-contrast h1,
    .high-contrast h2,
    .high-contrast h3,
    .high-contrast p,
    .high-contrast li,
    .high-contrast a {
      color: yellow;
    }

    .high-contrast button {
      background: yellow;
      color: black;
    }

    /* Daltonismo */

    .protanopia .color-red {
      color: #ffb3b3 !important;
    }

    .deuteranopia .color-green {
      color: #c8ffb0 !important;
    }

    .tritanopia .color-blue {
      color: #9ecbff !important;
    }

    .acromatopsia {
      filter: grayscale(100%);
    }

    @media (max-width: 768px) {

      .controls {
        position: static;
        width: 100%;
        margin-top: 20px;
      }

      header h1 {
        font-size: 2rem;
      }

      nav {
        padding: 10px;
      }
    }
  </style>
</head>

<body>

  <header>
    <h1>Site Acessível</h1>

    <p>
      Um projeto voltado para inclusão, acessibilidade digital
      e conscientização sobre deficiência visual.
    </p>
  </header>

  <nav aria-label="Menu principal">
    <a href="#acessibilidade">Acessibilidade</a>
    <a href="#digital">Digital</a>
    <a href="#dados">Dados</a>
    <a href="#assistivas">Tecnologias</a>
    <a href="#ia">IA</a>
    <a href="#educacao">Educação</a>
    <a href="#importancia">Importância</a>
  </nav>

  <main>

    <section class="section" id="acessibilidade">
      <h2>O que é Acessibilidade?</h2>

      <p>
        <span class="color-red">Acessibilidade</span> significa criar
        ambientes, produtos e serviços que possam ser utilizados
        por todas as pessoas.
      </p>

      <p>
        Isso inclui pessoas com deficiência física,
        visual, auditiva ou cognitiva.
      </p>

      <p>
        A acessibilidade promove autonomia,
        igualdade e inclusão social.
      </p>
    </section>

    <section class="section" id="digital">
      <h2>O que é Acessibilidade Digital?</h2>

      <p>
        <span class="color-green">Acessibilidade digital</span>
        consiste em desenvolver sites, aplicativos e sistemas
        acessíveis para todos os usuários.
      </p>

      <div class="cards">

        <div class="card">
          <h3>Leitores de Tela</h3>
          <p>
            Transformam textos em áudio para pessoas cegas.
          </p>
        </div>

        <div class="card">
          <h3>Alto Contraste</h3>
          <p>
            Facilita a leitura para pessoas com baixa visão.
          </p>
        </div>

        <div class="card">
          <h3>Navegação por Teclado</h3>
          <p>
            Permite usar o site sem mouse.
          </p>
        </div>

      </div>
    </section>

    <section class="section" id="dados">
      <h2>Deficiência Visual no Mundo</h2>

      <p>
        Mais de <span class="color-red">2,2 bilhões de pessoas</span>
        possuem algum tipo de deficiência visual.
      </p>

      <p>
        O <span class="color-green">daltonismo</span>
        afeta milhões de pessoas em todo o mundo.
      </p>

      <p>
        Mesmo assim, muitos sistemas continuam sendo criados
        sem considerar acessibilidade. A humanidade conseguiu
        criar inteligência artificial antes de aprender a fazer
        botão legível. Uma conquista curiosa.
      </p>
    </section>

    <section class="section" id="assistivas">
      <h2>Tecnologias Assistivas</h2>

      <p>
        Tecnologias assistivas ajudam pessoas com deficiência
        a utilizar computadores, celulares e plataformas digitais.
      </p>

      <div class="cards">

        <div class="card">
          <h3>Comandos de Voz</h3>
          <p>
            Permitem controlar dispositivos usando apenas a fala.
          </p>
        </div>

        <div class="card">
          <h3>Teclados Adaptados</h3>
          <p>
            Auxiliam pessoas com limitações motoras.
          </p>
        </div>

        <div class="card">
          <h3>Ampliadores de Tela</h3>
          <p>
            Aumentam conteúdos para pessoas com baixa visão.
          </p>
        </div>

      </div>
    </section>

    <section class="section" id="ia">
      <h2>Inteligência Artificial e Inclusão</h2>

      <p>
        A inteligência artificial vem sendo utilizada
        para melhorar a acessibilidade digital.
      </p>

      <ul>
        <li>Descrição automática de imagens</li>
        <li>Conversão de voz em texto</li>
        <li>Leitura inteligente de documentos</li>
        <li>Auxílio de navegação para deficientes visuais</li>
      </ul>

      <p>
        Quando usada corretamente, a IA pode reduzir barreiras
        e ampliar a inclusão social.
      </p>
    </section>

    <section class="section" id="educacao">
      <h2>Acessibilidade na Educação</h2>

      <p>
        A educação acessível é essencial para garantir
        igualdade de oportunidades.
      </p>

      <p>
        Muitos estudantes ainda enfrentam dificuldades
        para acessar plataformas digitais e materiais online.
      </p>

      <p>
        Ambientes educacionais acessíveis permitem maior
        autonomia, inclusão e desenvolvimento acadêmico.
      </p>
    </section>

    <section class="section" id="importancia">
      <h2>Por que isso importa?</h2>

      <p>
        Ignorar acessibilidade significa excluir pessoas
        da educação, do trabalho e da vida social.
      </p>

      <p>
        Pequenas adaptações podem transformar completamente
        a experiência de milhões de usuários.
      </p>

      <p>
        <span class="color-blue">
          A acessibilidade não é um luxo. É um direito.
        </span>
      </p>
    </section>

  </main>

  <div class="controls" aria-label="Ferramentas de acessibilidade">

    <div class="controls-title">
      Acessibilidade
    </div>

    <div class="buttons-grid">

      <button onclick="toggleContrast()" aria-label="Ativar alto contraste">
        Contraste
      </button>

      <button onclick="resetView()" aria-label="Resetar configurações">
        Resetar
      </button>

      <button onclick="setProtanopia()" aria-label="Modo protanopia">
        Protanopia
      </button>

      <button onclick="setDeuteranopia()" aria-label="Modo deuteranopia">
        Deuteranopia
      </button>

      <button onclick="setTritanopia()" aria-label="Modo tritanopia">
        Tritanopia
      </button>

      <button onclick="setAcromatopsia()" aria-label="Modo acromático">
        Acromático
      </button>

    </div>

    <div class="font-control">

      <label for="fontSlider">
        Tamanho do texto
      </label>

      <input
        type="range"
        id="fontSlider"
        min="16"
        max="40"
        value="16"
        aria-label="Controle de tamanho do texto"
      >

    </div>

  </div>

  <footer>
    <p>
      Desenvolvido por Victor • Projeto de Acessibilidade Digital
    </p>
  </footer>

  <script>

    const slider = document.getElementById('fontSlider');

    slider.addEventListener('input', function () {
      document.body.style.fontSize = slider.value + 'px';
    });

    function toggleContrast() {
      document.body.classList.toggle('high-contrast');
    }

    function setProtanopia() {
      clearModes();
      document.body.classList.add('protanopia');
    }

    function setDeuteranopia() {
      clearModes();
      document.body.classList.add('deuteranopia');
    }

    function setTritanopia() {
      clearModes();
      document.body.classList.add('tritanopia');
    }

    function setAcromatopsia() {
      clearModes();
      document.body.classList.add('acromatopsia');
    }

    function clearModes() {
      document.body.classList.remove(
        'protanopia',
        'deuteranopia',
        'tritanopia',
        'acromatopsia'
      );
    }

    function resetView() {

      document.body.className = '';

      document.body.style.fontSize = '16px';

      slider.value = 16;
    }

  </script>

</body>
</html>

