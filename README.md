# Dr. Gustavo Brasil — Perícia Judicial, Direito & Tecnologia

[![CamaraUX Score](https://img.shields.io/badge/CamaraUX%20Score-100%2F100-gold?style=for-the-badge)](DESIGN.md)
[![Acessibilidade](https://img.shields.io/badge/Acessibilidade-WCAG%202.2%20AAA-brightgreen?style=for-the-badge)](DESIGN.md)
[![Licença](https://img.shields.io/badge/Licen%C3%A7a-Propriet%C3%A1ria-navy?style=for-the-badge)](LICENSE)

Landing page de alta conversão, autoridade jurídica e sofisticação editorial para o **Dr. Gustavo Brasil** (Perito Judicial há 18 anos · 3.000+ laudos · OAB/MG · CREA), integrando assistência técnica processual ao ecossistema **123 Perito**.

---

## 🏛️ Destaques do Projeto

- **Estética Editorial Luxury Forense**: Bipolaridade cromática intencional — *Dark Realm* no Hero para solenidade e sobriedade de corte superior, e *Warm Alabaster Realm* no corpo para clareza probatória inspirada em papel pergaminho de autos e laudos autenticados.
- **Zero AI Slop**: Fotografia e arquitetura 100% alinhadas à realidade jurídica brasileira — Palácio da Justiça (TJSP com bandeira nacional), contratos de prestação de serviços com selos notariais paulistas, fotografias em microscopia óptica forense real e sem clichês estrangeiros (sem gavels ou bolinhas macOS).
- **Acessibilidade WCAG 2.2 Nível AAA**:
  - Contraste cromático auditado (> 16:1 para textos principais, > 5.1:1 para acentos no claro).
  - Anel de foco de teclado contextual (`:focus-visible` com 3px de contorno e 3px de offset).
  - Formulário com feedback acessível em tempo real (`role="status"`, `aria-live="polite"`), sem bloqueio por `alert()` nativo.
  - Skip-link funcional e touch targets >= 48px para mobile.
- **Motion System (GSAP 3 & ScrollTrigger)**:
  - Animações escalonadas de entrada, elevação suave de cards e contadores numéricos progressivos.
  - Degradação graciosa: renderização garantida mesmo se o JavaScript ou CDN estiverem indisponíveis.
  - Suporte completo a `prefers-reduced-motion: reduce`.
- **Integração do Ecossistema 123 Perito**:
  - Plantão WhatsApp com SLA de resposta em até 4 horas úteis.
  - Formação 123 Perito na Hotmart (mais de 1.000 alunos formados).
  - Plataforma SaaS com tabela de planos: **Starter (R$ 9,90/mês)**, **Pro (R$ 29,90/mês)** e **Premium (R$ 49,90/mês)** com 10 dias grátis no cartão.

---

## 🛠️ Tecnologias Utilizadas

- **Estrutura**: HTML5 Semântico com microdados Schema.org (`LegalService` & `FAQPage`).
- **Estilização**: Vanilla CSS com arquitetura de tokens DTCG 2025.10 e tipografia fluida via `clamp()`.
- **Tipografia**: Cinzel, Cormorant Garamond e Plus Jakarta Sans (Google Fonts).
- **Animações**: GSAP 3.12.5 + ScrollTrigger.
- **Design System & Auditoria**: [DESIGN.md](DESIGN.md) auditado com **Score CamaraUX 100/100**.

---

## 📂 Estrutura de Arquivos

```text
lp-gustavo-brasil/
├── assets/                          # Imagens forenses, cortesias e fotografias reais
│   ├── card_grafotecnica.jpg
│   ├── card_justitia.jpg
│   ├── card_tribunal.jpg
│   ├── gustavo_brasil_cutout.png
│   ├── gustavo_brasil_hero.png
│   ├── gustavo_brasil_microscopio.jpg
│   └── hero_bg.jpg
├── index.html                       # Aplicação principal otimizada
├── DESIGN.md                        # Design System formal e guia de tokens DTCG
├── robots.txt                       # Diretrizes para indexadores
├── sitemap.xml                      # Mapa do site indexável
└── README.md                        # Documentação técnica do repositório
```

---

## ⚖️ Conformidade e Direitos

© 2026 Dr. Gustavo Brasil · 123 Perito. Todos os direitos reservados.  
Informativo pericial e jurídico em estrita consonância com o Código de Ética e Disciplina da OAB e normas técnicas ABNT/IBAPE.
