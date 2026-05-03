<!DOCTYPE html>
<html lang="pt-PT">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rahman Brussolo | Solutions Architect & AI-Native Engineer</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap"
        rel="stylesheet">
    <style>
        :root {
            --primary: #0f172a;
            --accent: #2563eb;
            --accent-soft: #eff6ff;
            --glass: rgba(255, 255, 255, 0.85);
            --border: rgba(226, 232, 240, 0.8);
            --text-main: #1e293b;
            --text-muted: #64748b;
            --sidebar-bg: #f8fafc;
        }

        * {
            box-sizing: border-box;
            -webkit-print-color-adjust: exact;
            print-color-adjust: exact;
        }

        body {
            font-family: 'Inter', sans-serif;
            color: var(--text-main);
            background-color: #f1f5f9;
            margin: 0;
            padding: 20px 0;
            line-height: 1.6;
            letter-spacing: -0.01em;
        }

        .cv-page {
            max-width: 1000px;
            margin: 0 auto;
            background: white;
            border-radius: 24px;
            box-shadow: 0 40px 100px -20px rgba(0, 0, 0, 0.15);
            overflow: hidden;
            position: relative;
        }

        .hero-banner {
            width: 100%;
            height: 240px;
            background: var(--primary);
            position: relative;
        }

        .hero-banner img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            opacity: 0.9;
        }

        .header-card {
            position: absolute;
            top: 150px;
            left: 40px;
            right: 40px;
            background: var(--glass);
            backdrop-filter: blur(20px) saturate(160%);
            -webkit-backdrop-filter: blur(20px) saturate(160%);
            border: 1px solid rgba(255, 255, 255, 0.5);
            border-radius: 20px;
            padding: 20px 30px;
            display: flex;
            align-items: center;
            gap: 30px;
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.1);
            z-index: 10;
        }

        .profile-photo {
            width: 150px;
            height: 150px;
            border-radius: 16px;
            overflow: hidden;
            border: 4px solid white;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
            flex-shrink: 0;
            transform: translateY(-5px);
        }

        .profile-photo img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .header-text {
            flex: 1;
        }

        h1 {
            margin: 0;
            font-size: 2.6rem;
            font-weight: 800;
            letter-spacing: -1.8px;
            color: var(--primary);
            line-height: 1;
        }

        .tagline {
            font-size: 1.15rem;
            font-weight: 600;
            color: var(--accent);
            margin-top: 10px;
            letter-spacing: -0.4px;
        }

        .web-link {
            font-size: 0.75rem;
            margin-top: 8px;
        }

        .web-link a {
            color: var(--accent);
            text-decoration: none;
            font-weight: 500;
            display: inline-flex;
            align-items: center;
            gap: 5px;
            opacity: 0.8;
        }

        .web-link a:hover {
            text-decoration: underline;
            opacity: 1;
        }

        .content-layout {
            display: grid;
            grid-template-columns: 300px 1fr;
            margin-top: 100px;
        }

        .sidebar {
            background: var(--sidebar-bg);
            padding: 50px 35px 35px 35px;
            border-right: 1px solid var(--border);
        }

        .main-col {
            padding: 50px 45px 35px 45px;
        }

        section {
            margin-bottom: 40px;
        }

        .section-title {
            font-size: 0.8rem;
            font-weight: 800;
            text-transform: uppercase;
            letter-spacing: 1.8px;
            color: var(--text-muted);
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .section-title::after {
            content: "";
            flex: 1;
            height: 1px;
            background: var(--border);
        }

        .info-list {
            list-style: none;
            padding: 0;
            margin: 0 0 35px 0;
        }

        .info-list li {
            margin-bottom: 12px;
            font-size: 0.85rem;
            font-weight: 500;
            color: var(--text-main);
        }

        .btn-link {
            display: block;
            text-decoration: none;
            padding: 8px 12px;
            background: white;
            border: 1px solid var(--border);
            border-radius: 10px;
            margin-bottom: 8px;
            font-size: 0.8rem;
            font-weight: 700;
            color: var(--primary);
            transition: 0.2s;
            text-align: center;
        }

        .btn-link:hover {
            border-color: var(--accent);
            color: var(--accent);
            transform: translateX(3px);
        }

        .skill-box {
            margin-bottom: 25px;
        }

        .skill-box h4 {
            font-size: 0.7rem;
            color: var(--text-muted);
            text-transform: uppercase;
            margin-bottom: 10px;
        }

        .pills-container {
            display: flex;
            flex-wrap: wrap;
            gap: 6px;
        }

        .skill-pill {
            background: white;
            padding: 4px 10px;
            border-radius: 6px;
            font-size: 0.7rem;
            font-weight: 600;
            border: 1px solid var(--border);
        }

        .exp-timeline {
            border-left: 2px solid var(--border);
            padding-left: 25px;
            margin-left: 5px;
        }

        .exp-entry {
            position: relative;
            margin-bottom: 35px;
        }

        .exp-entry::before {
            content: "";
            position: absolute;
            left: -33px;
            top: 5px;
            width: 12px;
            height: 12px;
            border-radius: 50%;
            background: white;
            border: 3px solid var(--accent);
        }

        .exp-meta {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 6px;
        }

        .comp-name {
            font-size: 1.15rem;
            font-weight: 800;
            color: var(--primary);
            letter-spacing: -0.4px;
        }

        .comp-name a {
            color: var(--accent);
            text-decoration: none;
        }

        .exp-date {
            font-size: 0.75rem;
            font-weight: 700;
            color: var(--text-muted);
            background: var(--sidebar-bg);
            padding: 3px 8px;
            border-radius: 6px;
        }

        .role-name {
            font-size: 0.9rem;
            font-weight: 700;
            color: var(--text-main);
            margin-bottom: 10px;
            display: block;
        }

        .exp-list {
            padding-left: 18px;
            margin: 0;
        }

        .exp-list li {
            font-size: 0.9rem;
            margin-bottom: 6px;
            color: var(--text-main);
            text-align: justify;
        }

        .edu-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 10px;
        }

        .edu-card {
            padding: 12px;
            border-radius: 12px;
            border: 1px solid var(--border);
            background: var(--sidebar-bg);
        }

        .edu-card b {
            display: block;
            font-size: 0.85rem;
            color: var(--primary);
        }

        .edu-card span {
            font-size: 0.75rem;
            color: var(--text-muted);
        }

        .cv-footer {
            text-align: center;
            padding: 25px;
            font-size: 0.75rem;
            color: var(--text-muted);
            background: var(--sidebar-bg);
            border-top: 1px solid var(--border);
        }

        @media print {
            body {
                padding: 0;
                background: white;
            }

            .cv-page {
                border-radius: 0;
                box-shadow: none;
                max-width: 100%;
            }

            .hero-banner {
                height: 160px;
            }

            .header-card {
                top: 90px;
                background: white !important;
                backdrop-filter: none;
                border: 1px solid #ddd;
                padding: 15px 25px;
            }

            .sidebar {
                background: #fff !important;
                width: 280px;
            }

            .main-col {
                padding: 40px 30px;
            }

            section {
                margin-bottom: 30px;
            }

            @page {
                margin: 0;
                size: A4;
            }
        }
    </style>
</head>

<body>

    <div class="cv-page">

        <div class="hero-banner">
            <img src="Banner.png" alt="Engineering Banner">
        </div>

        <header class="header-card">
            <div class="profile-photo">
                <img src="Rahman.jpg" alt="Rahman Profile">
            </div>
            <div class="header-text">
                <h1>Rahman Brussolo</h1>
                <div class="tagline">Solutions Architect | Product Engineer AI-Native | OutSystems Expert 11/ODC</div>
                <div class="web-link">
                    <a href="https://thander21.github.io/Product-Engineer-AI-Native/" target="_blank">
                        <span>🌐 Versão Online:</span> thander21.github.io/Product-Engineer-AI-Native/
                    </a>
                </div>
            </div>
        </header>

        <div class="content-layout">

            <aside class="sidebar">

                <div class="section-title">Contatos</div>
                <ul class="info-list">
                    <li>📍 Barreiro, Portugal</li>
                    <li>📞 +351 966 006 569</li>
                    <li>✉️ rahman13@gmail.com</li>
                    <li>🌍 GMT+0 (Portugal)</li>
                </ul>

                <div class="section-title">Links</div>
                <a href="https://linkedin.com/in/rahman-brussolo" class="btn-link">LinkedIn</a>
                <a href="https://github.com/Thander21" class="btn-link">GitHub</a>
                <a href="https://www.outsystems.com/profile/lxzupejyhh/overview" class="btn-link">OutSystems
                    Community</a>
                <a href="https://rahman.portfolio.sampati.com.br" class="btn-link">Portfolio</a>

                <div style="margin-top: 30px;" class="section-title">Tech Stack</div>

                <div class="skill-box">
                    <h4>Low-Code Enterprise</h4>
                    <div class="pills-container">
                        <span class="skill-pill">OutSystems ODC & O11</span>
                        <span class="skill-pill">4-Layer Architecture</span>
                        <span class="skill-pill">Reactive / Mobile</span>
                        <span class="skill-pill">ERP Architecture</span>
                        <span class="skill-pill">APIs REST/SOAP</span>
                        <span class="skill-pill">Forge Expert</span>
                    </div>
                </div>

                <div class="skill-box">
                    <h4>AI & Automation</h4>
                    <div class="pills-container">
                        <span class="skill-pill">Agent Orchestration</span>
                        <span class="skill-pill">Antigravity / Claude AI</span>
                        <span class="skill-pill">n8n / Make.com</span>
                        <span class="skill-pill">Prompt Eng.</span>
                        <span class="skill-pill">Chatwoot</span>
                        <span class="skill-pill">AI Integration IDE</span>
                        <span class="skill-pill">Scripting / Shell / Python</span>
                    </div>
                </div>

                <div class="skill-box">
                    <h4>DevOps & SRE</h4>
                    <div class="pills-container">
                        <span class="skill-pill">CI/CD Automation</span>
                        <span class="skill-pill">PowerShell / Bash Script</span>
                        <span class="skill-pill">AWS / Supabase</span>
                        <span class="skill-pill">Docker / Coolify</span>
                        <span class="skill-pill">Zabbix / CyberArk</span>
                        <span class="skill-pill">IaC Fundamentals</span>
                    </div>
                </div>

                <div class="skill-box">
                    <h4>Polyglot Engineering</h4>
                    <div class="pills-container">
                        <span class="skill-pill">Flutter / Dart</span>
                        <span class="skill-pill">Python</span>
                        <span class="skill-pill">C# .NET</span>
                        <span class="skill-pill">Node.js / React</span>
                    </div>
                </div>

                <div class="section-title">Idiomas</div>
                <div class="edu-grid">
                    <div class="edu-card"><b>Português</b><span>Nativo</span></div>
                    <div class="edu-card"><b>Inglês</b><span>Intermediário (Profissional)</span></div>
                </div>

            </aside>

            <main class="main-col">

                <section>
                    <div class="section-title">Resumo Profissional</div>
                    <p style="text-align: justify; font-size: 0.95rem; color: #334155; margin-top: 0;">
                        Expert em <b>OutSystems (Certificado ODC/O11)</b> ancorado por <b>25 anos de estrada técnica e
                            estratégica</b>. Como ex-CEO, trago uma visão pragmática focada em ROI e resiliência — não
                        apenas escrevo código, desenho soluções que sustentam negócios. Atualmente, impulsiono a
                        <b>Engenharia de Produtos AI-Native e DevOps</b>, utilizando orquestração de agentes para
                        acelerar entregas complexas sem abrir mão da governança e da estabilidade de infraestrutura.
                    </p>
                </section>

                <section>
                    <div class="section-title">Experiência Profissional</div>
                    <div class="exp-timeline">

                        <div class="exp-entry">
                            <div class="exp-meta">
                                <span class="comp-name"><a href="https://vittasync.pt">VittaSync</a> | Projetos
                                    R&D</span>
                                <span class="exp-date">2025 — Presente</span>
                            </div>
                            <b class="role-name">Founder & Product Engineer AI-Native</b>
                            <ul class="exp-list">
                                <li><b>Agentic Orchestration</b>: Desenvolvimento de motores de orquestração via
                                    Antigravity e MCP para automação radical de infraestrutura.</li>
                                <li><b>Hybrid Infra & DevOps</b>: Gestão de infraestrutura própria (Linux/Windows) com
                                    foco em <b>Soberania de Dados</b>, operando Docker/Coolify e IIS com automação de
                                    CI/CD via GitHub Actions, Vercel e Cloudflare Pages.</li>
                                <li><b>Modern ERP Sync</b>: Arquitetura do <a href="https://pdvdmais.com.br">ERP PDV
                                        D+</a>, garantindo resiliência Offline-First e sincronia de dados em tempo real.
                                </li>
                                <li><b>Audit & Security Tooling</b>: Engenharia de agentes para auditoria profunda de
                                    código e mitigação de vulnerabilidades sistêmicas.</li>
                            </ul>
                        </div>

                        <div class="exp-entry">
                            <div class="exp-meta">
                                <span class="comp-name">NOS</span>
                                <span class="exp-date">2025 — Presente</span>
                            </div>
                            <b class="role-name">Especialista de Monitorização e Observabilidade de Infraestrutura</b>
                            <ul class="exp-list">
                                <li><b>High Availability Ops</b>: Arquitetura de observabilidade em larga escala (Stack
                                    Zabbix/Grafana/ELK), garantindo continuidade em serviços críticos de
                                    telecomunicações.</li>
                                <li><b>Incident Engineering</b>: Liderança técnica na resolução de incidentes complexos,
                                    focando na automação de alertas e redução drástica do MTTR através de cultura SRE.
                                </li>
                            </ul>
                        </div>

                        <div class="exp-entry">
                            <div class="exp-meta">
                                <span class="comp-name">Century21 PT/ES</span>
                                <span class="exp-date">2024 — 2025</span>
                            </div>
                            <b class="role-name">Knowledge Engineer & Tech Reliability Manager</b>
                            <ul class="exp-list">
                                <li><b>Knowledge Engineering</b>: Implementação de arquitetura de dados e conhecimento
                                    para suporte técnico em escala ibérica (PT/ES), reduzindo incidentes em 30%.</li>
                                <li><b>Operational Governance</b>: Automação estratégica de workflows para elevar a
                                    confiabilidade e o throughput dos serviços de suporte.</li>
                            </ul>
                        </div>

                        <div class="exp-entry">
                            <div class="exp-meta">
                                <span class="comp-name">Rodoxisto</span>
                                <span class="exp-date">2023 — 2024</span>
                            </div>
                            <b class="role-name">OutSystems Developer Fullstack (Arquiteto de Soluções Mobile)</b>
                            <ul class="exp-list">
                                <li><b>Cloud Integration Architecture</b>: Implementação de lógica resiliente para
                                    processamento de documentos (OCR) e armazenamento em AWS S3 via OutSystems.</li>
                                <li><b>Dynamic Security Engine</b>: Motor de permissões granulares via JSON, elevando o
                                    padrão de governança do produto.</li>
                                <li><b>Transição Estratégica</b>: Conclusão do ciclo na empresa motivada pela mudança
                                    para Portugal, mantendo entregas de alta qualidade, mesmo remoto part-time nos
                                    ultimos meses.</li>
                            </ul>
                        </div>

                        <div class="exp-entry">
                            <div class="exp-meta">
                                <span class="comp-name">B2Food</span>
                                <span class="exp-date">Ago 2023 — Nov 2023</span>
                            </div>
                            <b class="role-name">OutSystems Architect & Fullstack Developer (MVP Development)</b>
                            <ul class="exp-list">
                                <li><b>End-to-End Product Architecture</b>: Design e implementação integral do blueprint
                                    arquitetural do MVP, abrangendo modelagem de dados, lógica de negócio e padrões de
                                    comunicação para escala mobile.</li>
                                <li><b>Fullstack Implementation</b>: Desenvolvimento E2E de aplicação mobile reativa,
                                    garantindo uma UX de alta performance e integração fluida com camadas de backend e
                                    APIs externas.</li>
                                <li><b>Legacy Modernization</b>: Liderança na refatoração e redesenho de processos
                                    legados, otimizando fluxos de dados para reduzir a latência e aumentar a resiliência
                                    do ecossistema.</li>
                            </ul>
                        </div>

                        <div class="exp-entry">
                            <div class="exp-meta">
                                <span class="comp-name">PHNet</span>
                                <span class="exp-date">Jan 2023 — Jul 2023</span>
                            </div>
                            <b class="role-name">OutSystems Developer Senior & Network Automation</b>
                            <ul class="exp-list">
                                <li><b>Fullstack Network Orchestration</b>: Desenvolvimento de arquitetura E2E para
                                    gestão de infraestrutura ISP, integrando OutSystems com Radius e MikroTik para
                                    provisionamento e monitorização em tempo real.</li>
                                <li><b>Scalable Data Processing</b>: Otimização de processos assíncronos (Timers) para
                                    processamento massivo de logs de tráfego e métricas de autenticação, garantindo
                                    performance em larga escala.</li>
                                <li><b>Geographical Intelligence & UX</b>: Design de dashboards reativos complexos com
                                    visualização geográfica de incidentes críticos, elevando a eficiência das equipas de
                                    suporte nível 2 e 3.</li>
                                <li><b>API Governance</b>: Implementação de camadas de abstração (Service Actions/APIs)
                                    para isolamento de protocolos de rede e lógica de negócio.</li>
                            </ul>
                        </div>

                        <div class="exp-entry" style="margin-bottom: 0;">
                            <div class="exp-meta">
                                <span class="comp-name"><a href="https://sampati.com.br">Sampa TI</a></span>
                                <span class="exp-date">2012 — 2023</span>
                            </div>
                            <b class="role-name">CEO & Arquiteto de Soluções (Strategic Product Engineering)</b>
                            <ul class="exp-list">
                                <li><b>Strategic Evolution (11+ Anos)</b>: Trajetória completa de liderança, evoluindo
                                    de técnico de implantação e formação de equipas para a arquitetura total de sistemas
                                    e gestão executiva da empresa.</li>
                                <li><b>Fullstack Ecosystem Management</b>: Liderança técnica hands-on (C# / JS /
                                    OutSystems), garantindo a estabilidade e operação crítica de mais de 300 clientes
                                    enterprise.</li>
                                <li><b>Continuous Legacy Optimization</b>: Atuação contínua (atualmente via VittaSync)
                                    na modernização de todo o parque tecnológico construído, injetando automação DevOps
                                    e inteligência AI-Native para maximizar a resiliência e o ROI.</li>
                                <li><b>Business & Tech Bridge</b>: Tradução de necessidades complexas de negócio em
                                    soluções de software escaláveis, mantendo um suporte nível 3 de alta disponibilidade
                                    por mais de uma década.</li>
                            </ul>
                        </div>

                    </div>
                </section>

                <section style="margin-top: 40px;">
                    <div class="section-title">Formação e Certificações</div>
                    <div class="edu-grid" style="grid-template-columns: 1fr 1fr;">
                        <div class="edu-card"><b>Bacharelado Eng. Software</b><span>Unigra EAD (Foco em
                                Arquitetura)</span></div>
                        <div class="edu-card"><b>Tecnólogo Gestão TI</b><span>Fanor (Concluído em 2012)</span></div>
                        <div class="edu-card"><b>OutSystems Certified</b><span>Associate Reactive Developer</span></div>
                        <div class="edu-card"><b>Cibersegurança</b><span>Fundamentos SOC & Governança</span></div>
                    </div>
                </section>

                <section style="margin-top: 40px;">
                    <div class="section-title">Fundação Técnica (Hardcore Tech)</div>
                    <div class="edu-grid" style="grid-template-columns: 1fr 1fr;">
                        <div class="edu-card"><b>Solução Sistemas (2010 — 2012)</b><span>Coordenação técnica e
                                engenharia de implantação de ERPs.</span></div>
                        <div class="edu-card"><b>Setor Comercial & Logística (2007 — 2010)</b><span>Gestão estratégica
                                de compras e arquitetura de projetos técnicos.</span></div>
                        <div class="edu-card"><b>Tecnologia & E-commerce (2004 — 2006)</b><span>Técnico em RF e
                                infraestrutura crítica para vendas online.</span></div>
                        <div class="edu-card"><b>Blockbuster (2001 — 2004)</b><span>Gerente de Unidade e Gestão de
                                Operações de Varejo.</span></div>
                        <div class="edu-card"><b>Tech Informática (1995 — 2001)</b><span>Hardcore Hardware, Redes e
                                Webdesign pioneiro.</span></div>
                    </div>
                </section>

            </main>
        </div>

        <footer class="cv-footer">
            Disponível para Projetos Estratégicos & Consultoria de Alto Impacto.
            <br>
            <small>Ativo técnico AI-Native arquitetado com a expertise de Rahman Brussolo sob governança Antigravity
                Pro.</small>
        </footer>

    </div>

</body>

</html>
