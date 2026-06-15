# Cumulus Agentforce — Omnichannel Demo Portal

**Canonical demo** — use this repo only ([live portal](https://sacrich.github.io/cumulus-agentforce-portal/)).

Mortgage / first-time buyer story: Marcus & Emily · **APP-2847** · separate from Palonia.

| Channel | File |
|---------|------|
| Portal | `index.html` |
| Email | `agenticEmailCumulusEN.html` |
| Web | `agenticwebCumulusEN.html` |
| Mobile app | `agenticMobileCumulusEN.html` |
| WhatsApp | `agenticWhatsappCumulusMortgageEN.html` |
| Data Cloud | `fichaclienteCumulusEN.html` |

## Local

```bash
python3 -m http.server 8081
```

Open http://localhost:8081/

`assets/demo-base.js` fixes asset paths on GitHub Pages (`/cumulus-agentforce-portal/`) and locally.
