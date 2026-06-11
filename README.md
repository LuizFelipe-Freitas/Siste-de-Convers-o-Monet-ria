<div align="center">
  <h1>💰 Sistema Financeiro de Conversão Monetária</h1>
  <p><strong>Automação de Testes (QA) e Interface de Câmbio em Tempo Real</strong></p>
</div>

<br>

## 📝 Descrição do Projeto
Este projeto compõe o sistema de monitoramento cambial desenvolvido para o core de operações internacionais de uma Fintech. Ele é dividido em duas frentes:
1. **Frontend:** Uma interface Glassmorphism robusta e responsiva para o usuário final realizar conversões.
2. **Backend/QA:** Uma suíte de testes de integração automatizados que garantem a estabilidade, o tempo de resposta (SLA) e a integridade da API consumida (`ExchangeRate-API`).

A qualidade do software é garantida através de uma pipeline contínua (CI/CD) que roda validações de contrato de dados, tratamento de falhas e status HTTP.

---

## 🛠️ Stack Tecnológica

### Backend & Automação (QA)
* <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" width="16" height="16"> **Python 3.11:** Linguagem base da automação.
* <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pytest/pytest-original.svg" width="16" height="16"> **Pytest:** Framework de orquestração de testes.
* 🌐 **Requests:** Consumo de APIs RESTful.
* 📊 **Pytest-HTML:** Geração de relatórios gerenciais e visuais.

### Frontend
* <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" width="16" height="16"> **HTML5 & CSS3:** Semântica e design moderno.
* <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" width="16" height="16"> **Vanilla JS:** Processamento assíncrono (Fetch API).

### DevOps & CI/CD
* <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" width="16" height="16"> **GitHub Actions:** Pipeline de integração contínua automatizada.
* 🚀 **GitHub Pages:** Deploy dinâmico dos relatórios do Pytest.

---

## 📂 Estrutura de Diretórios

```text
projeto_qa_fintech/
│
├── .github/workflows/
│   └── qa_pipeline.yml    # Configuração da pipeline no Github Actions
├── api/
│   ├── __init__.py
│   └── client.py          # Módulo HTTP isolado para a ExchangeRate-API
├── tests/
│   ├── __init__.py
│   └── test_cambio.py     # Casos de teste automatizados
├── reports/               # Artefatos gerados localmente
├── requirements.txt       # Dependências de ambiente
├── pytest.ini             # Arquivo de configuração de markers e logs do Pytest
├── index.html             # Interface do usuário (SPA) para conversão
└── README.md              # Este documento