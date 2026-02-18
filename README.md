<p align="center">
  <img src="https://raw.githubusercontent.com/avp-protocol/spec/main/assets/avp-shield.svg" alt="AVP Shield" width="80" />
</p>

<h1 align="center">AVP Website</h1>

<p align="center">
  <strong>Documentation website for Agent Vault Protocol</strong><br>
  avp.dev (coming soon)
</p>

<p align="center">
  <a href="https://github.com/avp-protocol/website/actions"><img src="https://img.shields.io/github/actions/workflow/status/avp-protocol/website/deploy.yml?style=flat-square" alt="Deploy" /></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-Apache_2.0-blue?style=flat-square" alt="License" /></a>
</p>

---

## Overview

This repository contains the source code for the AVP documentation website. It provides:

- Protocol specification (rendered from markdown)
- Getting started guides
- Implementation tutorials
- API reference documentation
- Integration guides

## Tech Stack

- **Framework**: [Astro](https://astro.build/) with [Starlight](https://starlight.astro.build/)
- **Styling**: Tailwind CSS
- **Hosting**: GitHub Pages / Cloudflare Pages
- **Search**: Pagefind

## Development

### Prerequisites

- Node.js 18+
- pnpm (recommended) or npm

### Setup

```bash
# Clone the repository
git clone https://github.com/avp-protocol/website.git
cd website

# Install dependencies
pnpm install

# Start development server
pnpm dev
```

### Build

```bash
pnpm build
```

### Preview production build

```bash
pnpm preview
```

## Project Structure

```
website/
├── src/
│   ├── content/
│   │   ├── docs/
│   │   │   ├── getting-started/
│   │   │   ├── specification/
│   │   │   ├── implementations/
│   │   │   ├── integrations/
│   │   │   └── reference/
│   │   └── config.ts
│   ├── components/
│   ├── layouts/
│   └── pages/
├── public/
│   ├── assets/
│   └── favicon.svg
├── astro.config.mjs
└── package.json
```

## Content Structure

| Section | Description |
|---------|-------------|
| `/getting-started` | Quick start, installation, migration guides |
| `/specification` | Full protocol spec, rendered from source |
| `/implementations` | Language-specific implementation guides |
| `/integrations` | Framework integration tutorials |
| `/reference` | API reference, error codes, configuration |

## Contributing

### Adding Documentation

1. Create a new `.md` or `.mdx` file in the appropriate `src/content/docs/` subdirectory
2. Add frontmatter with title and description
3. Write content using MDX (Markdown + JSX)
4. Submit a PR

### Syncing Specification

The specification is synced from the [spec repo](https://github.com/avp-protocol/spec):

```bash
pnpm sync-spec
```

This fetches the latest `avp-spec-v*.md` and converts it to the website format.

## Deployment

The website is automatically deployed on push to `main`:

- **GitHub Pages**: https://avp-protocol.github.io/website
- **Custom domain**: https://avp.dev (when configured)

## License

Apache 2.0 — see [LICENSE](LICENSE).

---

<p align="center">
  <a href="https://github.com/avp-protocol/spec">Specification</a> ·
  <a href="https://github.com/avp-protocol/website/issues">Issues</a>
</p>
