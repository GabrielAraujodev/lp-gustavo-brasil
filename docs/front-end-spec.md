# Front-End Spec — LP Gustavo Brasil & 123 Perito
Versão: 1.0.0 | Data: 2026-10-03 | Autor: Uma (ux-design-expert) | Fonte: index.html + DESIGN.md v2.3.0 + README.md
Status: Draft para revisão | Score CamaraUX alvo: 100/100 | WCAG: 2.2 AAA

## 1. Objetivo
Landing page estática de alta conversão e autoridade forense com 2 funis:
- (A) Advogado → WhatsApp Plantão (SLA 4h úteis)
- (B) Perito aspirante/ativo → Formação Hotmart + SaaS 123perito.com.br/planos

## 2. Usuários / JTBD
### Advogado patronal
- Job: contratar assistência técnica urgente (quesitos, impugnação, parecer)
- CTA primário: `Solicitar Análise de Viabilidade Pericial →` → https://api.whatsapp.com/send/?phone=5534991948659
- Fluxo: Hero → Serviços → Workflow 4 passos → WhatsApp

### Perito aspirante
- Job: formação + nomeações + prospecção de bancas
- CTA: Formação Hotmart https://gustavobrasil5.hotmart.host/pagina-de-vendas-6e0d3631-c30b-48cf-b9fa-ed235b8c39d4
- Fluxo: Training → Platform → Planos

### Perito ativo
- Job: operação (CRM, agenda, DJEN, leads)
- CTA: `Ativar 10 Dias Grátis no Plano Pro →` → https://123perito.com.br/planos
- Planos oficiais intocáveis: Starter R$9,90 / Pro R$29,90 / Premium R$49,90

## 3. IA / Seções
1. Header sticky 78px, skip-link #main, nav, CTA plantão, status-dot
2. Hero Dark #080D14 grid 1.15fr/0.85fr, badge SLA, H1 #hero-heading, lead, .btn-gold + .btn-ghost-dark, trust-bar, retrato + tag OAB/MG
3. Ribbon 3 cards overlap -85px
4. Why + mosaico + quote-box dark + 4 feats
5. Stats bar 4 métricas (18 anos, 3000+ laudos, 1000+ alunos, 12+ estados)
6. Pillars 3 colunas
7. Services 5 cards + workflow dark 4 passos
8. Training 2 col + pills + card dark
9. Platform dark SaaS mock (sem bolinhas macOS) + 3 planos + banner CTA
10. FAQ accordion acessível (aria-expanded, aria-controls)
11. Decision 2 cards
12. Footer 4 col + newsletter (#newsletter-form, #newsletter-email, #newsletter-feedback[role=status], #newsletter-submit-btn) + Schema LegalService + FAQPage

## 4. Sistema Atômico
- Atoms: kicker, btn-gold/ghost/outline-gold min 48px, curriculum-pill, inputs
- Molecules: hero-actions, feat-card, scard, faq-item, plan-card
- Organisms: header, hero-grid, ribbon-grid, workflow-box, crm-mockup-frame, decision-grid, footer-grid
- Tokens DTCG: --bg-dark #080D14, --bg-light #FBF9F5, --gold-on-dark #DFC5A2, --gold-deep-accessible #78531C
- Foco :focus-visible 3px offset 3px (#DFC5A2 dark, #78531C light)
- Tipografia: Cinzel display, Cormorant editorial, Plus Jakarta body via clamp()

## 5. Estados / Motion
- Hover btn translateY(-2px), cards -5 a -8px, borda gold
- GSAP 3.12.5 + ScrollTrigger apenas enhance, immediateRender:false, visível sem JS
- Form: default → sending disabled → success #34D399 / error #EF4444 inline, nunca alert()
- Breakpoints: <640 1col, 641-1024 2col, 1025+ full

## 6. Integrações / SEO / Perf
- WhatsApp com texto contextual, Hotmart, /planos com UTM, rel=noopener
- Meta OG pt_BR, theme #080D14, robots/sitemap ok, alt BR real (sem gavel/US flag)
- Alvos: LCP <2.5s, CLS <0.1, contraste 17.2:1 dark / 16.5:1 light

## 7. Aceite
- [ ] Tab completo com anel visível
- [ ] Newsletter anuncia via aria-live=polite
- [ ] Mobile 360px sem overflow, targets ≥48px
- [ ] Links e preços corretos
- [ ] Sem JS legível, sem opacity:0 travado
