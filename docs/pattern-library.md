# Pattern Library — LP Gustavo Brasil & 123 Perito
Versão 1.0 | Atomic Design | WCAG AAA

## Atoms
- `.btn-gold` (CTA primário WhatsApp/Hotmart), `.btn-ghost-dark`, `.btn-outline-gold`, `.plan-btn-action.gold/ghost` — min-height 48px, uppercase 0.76-0.86rem, focus 3px
- `.kicker.dark-mode/light-mode`, `.curriculum-pill`, `.newsletter-input`, `.status-dot`
- Tokens: `--bg-dark #080D14`, `--bg-light #FBF9F5`, `--gold-on-dark #DFC5A2`, `--gold-deep-accessible #78531C`

## Molecules
- `hero-actions`, `trust-item`, `card-action-link`, `feat-card (.feat-icon-box + .feat-info)`, `scard (.scard-num + h3 + p + .scard-tag)`, `faq-item (.faq-question-btn + .faq-answer-panel)`, `plan-card (.plan-name + .plan-price-box + .plan-features-list + CTA)`

## Organisms
- `site-header` sticky 78px, `hero-grid 1.15/0.85`, `ribbon-grid 3col`, `why-grid`, `stats-grid 4col`, `pillars-grid 3col`, `workflow-box dark`, `training-grid`, `crm-mockup-frame (topbar + body-grid 3col)`, `plans-grid 3col (featured Pro)`, `faq-accordion-list max 840px`, `decision-grid 2col`, `footer-grid 4col`

## Templates/Pages
- Dark Realm: hero, stats-bar, workflow-box, platform, footer
- Light Alabaster: ribbon, why, pillars, services, training, faq, decision

## Regras
- Nunca token primitivo direto no componente, usar semântico
- Preservar IDs: #main #hero-heading #newsletter-form #newsletter-email #newsletter-feedback #newsletter-submit-btn #faq-btn-*
- Proibido: alert(), outline:none sem substituto, gavel/US flag, bolinhas macOS, opacity:0 travado
- Motion: GSAP enhance only, immediateRender:false, reduced-motion respected
