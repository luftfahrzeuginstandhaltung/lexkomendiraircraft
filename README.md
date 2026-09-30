<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>AK-ARANY SAS | Biblioteca Técnica - LexKomendirCompanyAirCraft</title>
  <link rel="canonical" href="https://luftfahrzeuginstandhaltung.github.io/lexkomendiraircraft/biblioteca.html">
  <meta name="description" content="Biblioteca Técnica AK-ARANY SAS - Acervo RBAC 21, UL350iS 130HP, compósitos Berkut 360 - LexKomendirCompanyAirCraft - Fase conceitual 2026">
  <meta property="og:title" content="AK-ARANY SAS | Biblioteca Técnica">
  <meta property="og:description" content="Acervo para estudo de engenharia - RBAC 21, UL350iS, Berkut 360">
  
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;900&family=JetBrains+Mono:wght@400;700&display=swap" rel="stylesheet">
  
  <style>
    :root {
      --fundo: #020a18;
      --ouro: #d4af37;
      --ouro-claro: #f0d78c;
      --texto: #e5e7eb;
      --texto-claro: #94a3b8;
      --barra: #0f1e3a;
      --aba-ativa: #1e3a5f;
      --borda: #1e3a5f;
      --aviso-amarelo: rgba(234, 179, 8, 0.08);
      --etiqueta-verde: rgba(34, 197, 94, 0.15);
      --etiqueta-vermelho: rgba(239, 68, 68, 0.15);
    }
    
    * { margin: 0; padding: 0; box-sizing: border-box; }
    
    body { 
      background: var(--fundo); 
      color: var(--texto); 
      font-family: 'Inter', system-ui, -apple-system, sans-serif; 
      line-height: 1.6; 
      display: flex; 
      flex-direction: column; 
      min-height: 100vh; 
    }
    
    a { color: var(--ouro); text-decoration: none; transition: color .2s; }
    a:hover { color: var(--ouro-claro); }
    
    header { 
      background: var(--barra); 
      border-bottom: 1px solid var(--borda); 
      padding: 1rem 2rem; 
      display: flex; 
      justify-content: space-between; 
      align-items: center; 
      position: sticky; 
      top: 0; 
      z-index: 100; 
    }
    
    .logo { 
      font-weight: 900; 
      font-size: 1.25rem; 
      letter-spacing: .05em; 
      color: var(--ouro); 
      display: flex; 
      align-items: center; 
      gap: .5rem; 
    }
    
    nav ul { display: flex; list-style: none; gap: 1.5rem; }
    nav a { font-size: .9rem; font-weight: 500; color: var(--texto-claro); }
    nav a:hover, nav a.active { color: var(--ouro); }
    
    main { flex: 1; max-width: 1200px; width: 100%; margin: 2rem auto; padding: 0 1.5rem; }
    
    .notice-banner { 
      background: var(--aviso-amarelo); 
      border: 1px solid rgba(234, 179, 8, 0.3); 
      border-radius: 8px; 
      padding: 1rem; 
      margin-bottom: 2rem; 
      display: flex; 
      align-items: center; 
      gap: 1rem; 
      font-size: 0.875rem; 
    }
    .notice-banner strong { color: var(--ouro-claro); }
    
    .search-section { 
      background: rgba(15, 30, 58, 0.5); 
      border: 1px solid var(--borda); 
      border-radius: 8px; 
      padding: 1.5rem; 
      margin-bottom: 2rem; 
    }
    .search-box { display: flex; gap: 1rem; margin-bottom: 1rem; }
    .search-box input { 
      flex: 1; 
      background: var(--fundo); 
      border: 1px solid var(--borda); 
      color: var(--texto); 
      padding: .75rem 1rem; 
      border-radius: 6px; 
      font-family: inherit; 
      font-size: 1rem; 
    }
    .search-box input:focus { outline: none; border-color: var(--ouro); }
    .search-box button { 
      background: var(--ouro); 
      color: var(--fundo); 
      border: none; 
      padding: .75rem 1.5rem; 
      border-radius: 6px; 
      font-weight: 700; 
      cursor: pointer; 
    }
    .search-box button:hover { background: var(--ouro-claro); }
    
    .filter-tags { display: flex; flex-wrap: wrap; gap: .5rem; }
    .tag { 
      background: var(--barra); 
      border: 1px solid var(--borda); 
      color: var(--texto-claro); 
      padding: .25rem .75rem; 
      border-radius: 20px; 
      font-size: .8rem; 
      cursor: pointer; 
      transition: all .2s; 
    }
    .tag:hover, .tag.active { background: var(--aba-ativa); color: var(--ouro); border-color: var(--ouro); }
    
    .doc-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(340px, 1fr)); gap: 1.5rem; }
    .doc-card { 
      background: var(--barra); 
      border: 1px solid var(--borda); 
      border-radius: 8px; 
      padding: 1.5rem; 
      display: flex; 
      flex-direction: column; 
      justify-content: space-between; 
      transition: transform .2s, border-color .2s; 
    }
    .doc-card:hover { transform: translateY(-2px); border-color: var(--ouro); }
    
    .doc-header { display: flex; justify-content: space-between; align-items: flex-start; margin-bottom: .75rem; }
    .doc-code { 
      font-family: 'JetBrains Mono', 'Consolas', monospace; 
      font-size: .75rem; 
      color: var(--ouro); 
      background: rgba(212, 175, 55, 0.1); 
      padding: .2rem .5rem; 
      border-radius: 4px; 
    }
    .doc-status { font-size: .7rem; padding: .2rem .5rem; border-radius: 4px; text-transform: uppercase; font-weight: 700; }
    .status-active { background: var(--etiqueta-verde); color: #4ade80; }
    .status-draft { background: var(--aviso-amarelo); color: #facc15; }
    
    .doc-title { font-size: 1.1rem; font-weight: 700; margin-bottom: .5rem; color: var(--texto); }
    .doc-description { font-size: .875rem; color: var(--texto-claro); margin-bottom: 1rem; flex-grow: 1; }
    .doc-footer { 
      display: flex; 
      justify-content: space-between; 
      align-items: center; 
      border-top: 1px solid rgba(255, 255, 255, 0.05); 
      padding-top: 1rem; 
      font-size: .8rem; 
      color: var(--texto-claro); 
      margin-top: auto; 
    }
    
    .svg-container { 
      background: #020a18; 
      border: 1px solid #1e3a5f; 
      border-radius: 6px; 
      padding: 0.5rem; 
      margin-bottom: 0.75rem; 
      text-align: center; 
    }
    .svg-label { 
      font-size: 0.7rem; 
      color: var(--ouro-claro); 
      font-weight: 700; 
      display: block; 
      margin-bottom: 0.25rem; 
      text-transform: uppercase; 
      letter-spacing: 0.05em; 
    }
    
    .no-results { grid-column: 1 / -1; text-align: center; padding: 2rem; color: var(--texto-claro); display: none; }
    footer { background: var(--barra); border-top: 1px solid var(--borda); padding: 2rem; text-align: center; font-size: 0.8rem; color: var(--texto-claro); margin-top: auto; }
  </style>
</head>
<body>

  <header>
    <div class="logo">
      <span>AK-ARANY SAS</span>
    </div>
    <nav>
      <ul>
        <li><a href="index.html">Início</a></li>
        <li><a href="biblioteca.html" class="active">Biblioteca Técnica</a></li>
      </ul>
    </nav>
  </header>

  <main>
    <div class="notice-banner">
      <span>⚠️</span>
      <div>
        <strong>Aviso Institucional (Fase Conceitual 2026):</strong> Este acervo reúne estudos para desenvolvimento de engenharia aeronáutica. Referências a órgãos públicos (FINEP/BNDES) ou normas regulatórias (ANAC RBAC 21 / IS 21.191) possuem caráter exclusivamente acadêmico e de planejamento técnico.
      </div>
    </div>

    <section class="search-section">
      <div class="search-box">
        <input type="text" id="searchInput" placeholder="Buscar por título, código ou palavra-chave (ex: RBAC, UL350iS, Canard)...">
        <button id="searchBtn">Buscar</button>
      </div>
      <div class="filter-tags" id="filterTags">
        <span class="tag active" data-filter="all">Todos</span>
        <span class="tag" data-filter="regulatorio">Regulatório & ANAC</span>
        <span class="tag" data-filter="propulsao">Propulsão & UL350iS</span>
        <span class="tag" data-filter="estrutura">Estrutura & Compósitos</span>
        <span class="tag" data-filter="desenho">Desenhos Técnicos</span>
      </div>
    </section>

    <div class="doc-grid" id="docGrid">
      
      <!-- Documento 1 -->
      <article class="doc-card" data-category="regulatorio">
        <div>
          <div class="doc-header">
            <span class="doc-code">DOC-REG-001</span>
            <span class="doc-status status-active">Ativo</span>
          </div>
          <h2 class="doc-title">Diretrizes de Certificação Experimental (RBAC 21 / IS 21.191)</h2>
          <p class="doc-description">Análise detalhada do processo de obtenção do CAVE (Certificado de Autorização de Voo Experimental) para aeronaves de construção amadora.</p>
        </div>
        <div class="doc-footer">
          <span>Categoria: Regulatório</span>
          <a href="#">Acessar Documento &rarr;</a>
        </div>
      </article>

      <!-- Documento 2 -->
      <article class="doc-card" data-category="propulsao">
        <div>
          <div class="doc-header">
            <span class="doc-code">DOC-ENG-350</span>
            <span class="doc-status status-active">Ativo</span>
          </div>
          <h2 class="doc-title">Manual de Integração do Motor ULPower UL350iS (130HP)</h2>
          <p class="doc-description">Especificações técnicas de instalação, linhas de combustível, ECU FADEC e arrefecimento para a motorização da plataforma Berkut 360.</p>
        </div>
        <div class="doc-footer">
          <span>Categoria: Propulsão</span>
          <a href="#">Acessar Documento &rarr;</a>
        </div>
      </article>

      <!-- Documento 3 -->
      <article class="doc-card" data-category="estrutura">
        <div>
          <div class="doc-header">
            <span class="doc-code">DOC-MAT-012</span>
            <span class="doc-status status-draft">Rascunho</span>
          </div>
          <h2 class="doc-title">Especificação de Compósitos: Fibra de Carbono e Epóxi</h2>
          <p class="doc-description">Manual de procedimentos de cura, laminação em vácuo e controle de qualidade estrutural para componentes da asa e canard.</p>
        </div>
        <div class="doc-footer">
          <span>Categoria: Estrutura</span>
          <a href="#">Acessar Documento &rarr;</a>
        </div>
      </article>

      <!-- Documento 4 (Com Vetor Planta) -->
      <article class="doc-card" data-category="desenho">
        <div>
          <div class="doc-header">
            <span class="doc-code">DOC-DWG-001</span>
            <span class="doc-status status-active">Ativo</span>
          </div>
          <h2 class="doc-title">Esquema Geométrico de Planta - Arquitetura Canard</h2>
          <div class="svg-container">
            <span class="svg-label">Vista em Planta (Superior)</span>
            <svg viewBox="0 0 400 160" width="100%" height="auto" xmlns="http://www.w3.org/2000/svg">
              <path d="M 0,0 L 400,0 L 400,160 L 0,160 Z" fill="#020a18" />
              <!-- Canard Dianteiro -->
              <polygon points="100,72 130,50 145,50 135,72 135,88 145,110 130,110 100,88" fill="none" stroke="#d4af37" stroke-width="1.5"/>
              <!-- Fuselagem -->
              <path d="M 70,80 Q 120,65 220,68 L 310,72 L 310,88 L 220,92 Q 120,95 70,80 Z" fill="none" stroke="#d4af37" stroke-width="2"/>
              <!-- Canopy -->
              <path d="M 140,73 Q 180,68 220,73 Q 180,87 140,87 Z" fill="rgba(212,175,55,0.15)" stroke="#f0d78c" stroke-width="1"/>
              <!-- Asa Principal Traseira -->
              <polygon points="230,70 330,10 360,10 320,70 320,90 360,150 330,150 230,90" fill="none" stroke="#d4af37" stroke-width="1.5"/>
              <!-- Hélice Pusher -->
              <line x1="318" y1="55" x2="318" y2="105" stroke="#f0d78c" stroke-width="2" stroke-dasharray="2,2"/>
              <!-- Linha de Centro -->
              <line x1="50" y1="80" x2="370" y2="80" stroke="#1e3a5f" stroke-width="1" stroke-dasharray="4,4"/>
            </svg>
          </div>
          <p class="doc-description">Desenho vetorial de referência com enflechamento da asa, posicionamento do canard dianteiro e hélice traseira (pusher).</p>
        </div>
        <div class="doc-footer">
          <span>Categoria: Desenho Técnico</span>
          <a href="#">Acessar Documento &rarr;</a>
        </div>
      </article>

      <!-- Documento 5 (Com Vetor Perfil) -->
      <article class="doc-card" data-category="desenho">
        <div>
          <div class="doc-header">
            <span class="doc-code">DOC-DWG-002</span>
            <span class="doc-status status-active">Ativo</span>
          </div>
          <h2 class="doc-title">Esquema de Perfil Lateral e Trem de Pouso Triciclo</h2>
          <div class="svg-container">
            <span class="svg-label">Vista de Perfil (Lateral)</span>
            <svg viewBox="0 0 400 140" width="100%" height="auto" xmlns="http://www.w3.org/2000/svg">
              <path d="M 0,0 L 400,0 L 400,140 L 0,140 Z" fill="#020a18" />
              <!-- Solo -->
              <line x1="30" y1="120" x2="370" y2="120" stroke="#1e3a5f" stroke-width="1.5" stroke-dasharray="4,2"/>
              <!-- Perfil Fuselagem -->
              <path d="M 50,90 C 90,85 130,55 210,60 C 270,63 320,70 340,85 L 340,95 L 290,100 C 200,102 110,100 50,90 Z" fill="none" stroke="#d4af37" stroke-width="2"/>
              <!-- Canopy -->
              <path d="M 120,70 C 150,50 200,50 230,62" fill="none" stroke="#f0d78c" stroke-width="1.5"/>
              <!-- Canard Lateral -->
              <line x1="80" y1="88" x2="110" y2="86" stroke="#d4af37" stroke-width="2"/>
              <!-- Trem Bequilha Dianteiro -->
              <line x1="100" y1="94" x2="95" y2="114" stroke="#94a3b8" stroke-width="2"/>
              <circle cx="95" cy="114" r="5" fill="#d4af37"/>
              <!-- Trem Principal -->
              <line x1="250" y1="100" x2="255" y2="114" stroke="#94a3b8" stroke-width="2"/>
              <circle cx="255" cy="114" r="6" fill="#d4af37"/>
              <!-- Hélice Pusher -->
              <line x1="344" y1="65" x2="344" y2="105" stroke="#f0d78c" stroke-width="2"/>
            </svg>
          </div>
          <p class="doc-description">Visão em elevação demonstrando a linha de centro, Canopy tândem e distribuição de carga no trem de pouso.</p>
        </div>
        <div class="doc-footer">
          <span>Categoria: Desenho Técnico</span>
          <a href="#">Acessar Documento &rarr;</a>
        </div>
      </article>

      <div class="no-results" id="noResults">
        Nenhum documento encontrado com os critérios de busca especificados.
      </div>

    </div>
  </main>

  <footer>
    <p>&copy; 2026 LexKomendir Company AirCraft / AK-ARANY SAS. Todos os direitos reservados.</p>
    <p style="margin-top: 0.5rem; color: #64748b; font-size: 0.75rem;">Desenvolvimento de Engenharia Aeronáutica Conceitual - Berkut 360</p>
  </footer>

  <script>
    document.addEventListener('DOMContentLoaded', () => {
      const searchInput = document.getElementById('searchInput');
      const searchBtn = document.getElementById('searchBtn');
      const filterTags = document.querySelectorAll('.filter-tags .tag');
      const docCards = document.querySelectorAll('.doc-card');
      const noResults = document.getElementById('noResults');

      let currentFilter = 'all';

      function filterDocs() {
        const query = searchInput.value.toLowerCase().trim();
        let visibleCount = 0;

        docCards.forEach(card => {
          const category = card.getAttribute('data-category');
          const title = card.querySelector('.doc-title').textContent.toLowerCase();
          const desc = card.querySelector('.doc-description').textContent.toLowerCase();
          const code = card.querySelector('.doc-code').textContent.toLowerCase();

          const matchesCategory = (currentFilter === 'all' || category === currentFilter);
          const matchesQuery = (title.includes(query) || desc.includes(query) || code.includes(query));

          if (matchesCategory && matchesQuery) {
            card.style.display = 'flex';
            visibleCount++;
          } else {
            card.style.display = 'none';
          }
        });

        if (visibleCount === 0) {
          noResults.style.display = 'block';
        } else {
          noResults.style.display = 'none';
        }
      }

      filterTags.forEach(tag => {
        tag.addEventListener('click', () => {
          filterTags.forEach(t => t.classList.remove('active'));
          tag.classList.add('active');
          currentFilter = tag.getAttribute('data-filter');
          filterDocs();
        });
      });

      searchBtn.addEventListener('click', filterDocs);
      searchInput.addEventListener('keyup', (e) => {
        if (e.key === 'Enter') {
          filterDocs();
        } else {
          filterDocs();
        }
      });
    });
  </script>
</body>
</html>
