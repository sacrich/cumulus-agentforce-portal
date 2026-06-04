# Personalización de la demo Cumulus (banca / hipotecas)

Proyecto **paralelo** a `palonia-demo/` — misma mecánica omnicanal (Email → Web adaptativa → WhatsApp → Data Cloud 360 → Marketing Intelligence), con narrativa de **primera hipoteca** para [Cumulus Financial Services](https://cumulusfinserv.com/).

## Estructura

```
WORLD TOUR - TLV 2026/
├── palonia-demo/          ← demo hotel (no tocar)
└── cumulus-demo/
    ├── index.html
    ├── agenticEmailCumulusEN.html
    ├── agenticwebCumulusEN.html
    ├── agenticWhatsappCumulusMortgageEN.html
    ├── fichaclienteCumulusEN.html
    ├── marketingIntelligenceCumulusEN.html
    ├── CUSTOMIZACION.md
    └── assets/
        ├── cumulus-logo.png
        ├── cumulus-icon.png
        ├── cumulus-hero.jpg
        ├── cumulus-premier-card.svg
        └── agentforce_icon.webp
```

Hub: `/Users/sacrich/Desktop/WORLD TOUR - TLV 2026/cumulus-demo/index.html`

## Servidor local

```bash
cd "/Users/sacrich/Desktop/WORLD TOUR - TLV 2026/cumulus-demo"
python3 -m http.server 8081
```

Abre **http://localhost:8081/** (usa 8081 si 8080 está ocupado por Palonia).

## Historia de demo

| Elemento | Valor |
|----------|--------|
| Cliente | Marcus Thompson (+ Emily, co-borrower) |
| Caso | APP-2847 |
| Pre-calificación | Rango **$400K–$450K** (Austin) — sin propiedad fija en la demo |
| Programa | Conventional 30-year (email) |
| Promos | CUMULUS26 (-0.25%), RATELOCK48 (48h lock + fee waiver) |
| Canales | Email Agent → Adaptive Web → WhatsApp |

## Qué personalizar

1. **Marca** — Sustituye PNG/SVG en `assets/` o rutas en HTML. Logo oficial: `https://cumulus-fs.s3.amazonaws.com/images/cumulus-logo.png`
2. **Cliente** — Busca `Marcus` / `Emily` en los cinco HTML
3. **Caso e importes** — `APP-2847`, `$425,000`, tasas 6.25% / 6.125%
4. **Colores** — Navy `#0B3D5C`, teal `#00A3A1`
5. **Guion Agentforce** — Transcripciones en `fichaclienteCumulusEN.html`
6. **MI** — Campañas y atribución en `marketingIntelligenceCumulusEN.html`

## Flujo de presentación

1. **index.html** — contexto Cumulus / hipoteca
2. **Email** — campaña Path to Homeownership, cualificación
3. **Web** — borrador APP-2847, widgets adaptativos (calculadora, docs, seguro)
4. **WhatsApp** — resumen, Emily, nudge RATELOCK48
5. **Ficha cliente** — 360 + sesiones
6. **Marketing Intelligence** — ROI campañas mortgage

## Internet

CDN: React, Tailwind, Font Awesome, Google Fonts. Imágenes Unsplash en web/ficha. Assets Cumulus en `assets/` para logo y hero offline.
