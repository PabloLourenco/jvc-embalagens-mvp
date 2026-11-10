# Sistema de Controle de Fluxo e Conferência de Notas - JVC Embalagens

MVP desenvolvido como parte das práticas acadêmicas de Análise e Desenvolvimento de Sistemas (ADS).

## 📌 Contexto e Problema Comunitário
A **JVC Embalagens** é um pequeno empreendimento especializado na montagem e embalagem de componentes de fechaduras e ferragens. O projeto soluciona o gargalo de conferência manual de notas fiscais de entrada e saída, erradicando paradas na esteira de montagem e divergências de estoque físico em remessas industriais.

## 🎯 Vínculo com os Objetivos de Desenvolvimento Sustentável (ODS)
- **ODS 8 – Trabalho Decente e Crescimento Econômico** (Metas 8.2 e 8.3)
- Foco em elevar a produtividade por modernização técnica, eliminando o estresse do retrabalho e protegendo a sustentabilidade financeira do microempreendimento local.

## 🛠️ Tecnologias Utilizadas
- **Linguagem Principal:** Python 3.12
- **Framework Web Backend:** FastAPI
- **ORM / Persistência:** SQLAlchemy
- **Banco de Dados:** SQLite (embarcado/local) com suporte arquitetural a PostgreSQL
- **Frontend / Interface:** HTML5, CSS3 (Bootstrap 5) e JavaScript Vanilla (Progressive Web Application - PWA)
- **Extração Fiscal:** xmltodict / ElementTree para parsing de NF-e

## 🚀 Arquitetura e Estrutura Lógica
Arquitetura Monolítica em Camadas (Layered Architecture):
1. **Camada de Apresentação:** Interface web responsiva acessível no navegador da bancada de conferência e dispositivos móveis (alto contraste e alvos de toque de 44x44px).
2. **Camada de Negócio (Serviços):** Validação de regras fiscais, processamento assíncrono de XML e saldo de montagem.
3. **Camada de Persistência:** Modelagem relacional normalizada (`remessas_entrada` e `itens_remessa`).

## 📋 Status do Projeto
- [x] Diagnóstico Comunitário e Mapeamento de Dores
- [x] Modelagem Simplificada de Banco de Dados e Requisitos
- [x] Prototipação das 3 Telas Centrais do Fluxo
- [ ] Validação em Campo com Representante Externo
