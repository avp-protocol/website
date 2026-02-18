<p align="center">
  <img src="assets/avp-icon.svg" alt="AVP" width="80" />
</p>

<h1 align="center">AVP Protocol Website</h1>

<p align="center">
  <strong>Official website for Agent Vault Protocol</strong><br>
  <a href="https://avp-protocol.github.io/website">avp-protocol.github.io/website</a>
</p>

<p align="center">
  <a href="https://github.com/avp-protocol/website/actions"><img src="https://img.shields.io/github/actions/workflow/status/avp-protocol/website/deploy.yml?style=flat-square" alt="Deploy" /></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-Apache_2.0-blue?style=flat-square" alt="License" /></a>
</p>

---

## Overview

Static website for the Agent Vault Protocol ecosystem. Features:

- Protocol overview and features
- Implementation showcase (Python, TypeScript, Rust, Go)
- Framework integrations (LangChain, CrewAI, ZeroClaw)
- NexusClaw hardware product announcement

## Structure

```
website/
├── index.html          # Main landing page
├── css/
│   └── style.css       # Styles
├── js/
│   └── main.js         # JavaScript
├── assets/
│   ├── avp-logo.svg    # Logo
│   ├── avp-icon.svg    # Favicon
│   └── nexusclaw-device.svg
├── img/
│   ├── python.svg      # Language icons
│   ├── typescript.svg
│   ├── rust.svg
│   └── go.svg
└── .github/
    └── workflows/
        └── deploy.yml  # GitHub Pages deployment
```

## Development

Simply open `index.html` in a browser, or use a local server:

```bash
# Python
python -m http.server 8000

# Node.js
npx serve .
```

## Deployment

The website automatically deploys to GitHub Pages on push to `main`.

**Live URL:** https://avp-protocol.github.io/website

## Adding Pages

1. Create new `.html` file
2. Link from `index.html`
3. Push to `main`

## License

Apache 2.0 — see [LICENSE](LICENSE).

---

<p align="center">
  <a href="https://github.com/avp-protocol/spec">Specification</a> ·
  <a href="https://github.com/avp-protocol">GitHub</a>
</p>
