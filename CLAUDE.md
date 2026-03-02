# SpeedyPage Documentation

## About this project

Documentation site for SpeedyPage, built on [Mintlify](https://mintlify.com).

SpeedyPage is a cloud hosting provider offering web hosting, WordPress hosting, reseller hosting, VPS servers, and CDN services across seven global data center locations. UK-based, with 24/7 UK-based support as a core differentiator.

Audience: Small-to-medium business owners, WordPress users, developers/sysadmins, hosting resellers, and agencies. Mix of technical and non-technical readers — write for clarity without over-simplifying.

## Terminology

- **SpeedyPage** — one word, capital S capital P. Never "Speedy Page" or "speedypage"
- **Web Hosting** — shared/cPanel hosting product (not "shared hosting")
- **WordPress Hosting** — optimized WordPress product
- **Reseller Hosting** — white-label reseller product
- **Virtual Servers** or **NVMe VPS** — VPS product
- **CDN** — content delivery network product (powered by Bunny.net)
- Plan tiers: **Starter**, **Premium**, **Enterprise** (shared/WordPress/reseller products)
- **cPanel** — control panel for shared, WordPress, and reseller hosting
- **VirtFusion** — control panel for VPS
- **LiteSpeed** — web server (not Apache or Nginx)
- **NVMe SSD** — storage technology (sometimes "Gen4 NVMe")
- Data centers by city name: London, Ashburn, Los Angeles, Amsterdam, Singapore, Tokyo, Sydney
- Customer portal: **my.speedypage.com**

## Working relationship

- Push back on ideas when you have a better approach — cite sources and explain your reasoning
- Ask for clarification rather than making assumptions
- Never guess, fabricate, or hallucinate information

## How this repo is organized

- `docs.json` — Mintlify config: navigation, theme, colors, links. Validate changes against the [docs.json schema](https://mintlify.com/docs.json)
- `snippets/` — Reusable MDX content shared across pages
- `drafts/` and `*.draft.mdx` — Excluded from builds via `.mintignore`
- `images/` — PNG assets; `logo/` — SVG logos (light/dark variants)
- `api-reference/openapi.json` — OpenAPI spec for auto-generated endpoint docs

## Writing and style

Follow the guidelines in CONTRIBUTING.md and AGENTS.md. Key additions:

- Check existing pages for patterns before writing new content
- Use `snippets/` for content that appears on multiple pages
- Mintlify components in use: `<Card>`, `<CardGroup>`, `<Columns>`, `<Accordion>`, `<AccordionGroup>`, `<Tip>`, `<Note>`, `<Warning>`, `<CodeGroup>`
- Language tags on all code blocks, alt text on all images
- Relative paths for internal links (never absolute URLs)

## Content strategy

- Document just enough for user success — not too much, not too little
- Search for existing content before adding anything new
- Start by making the smallest reasonable change
- Make content evergreen when possible

## Development

- `mint dev` — Preview locally at http://localhost:3000
- `mint broken-links` — Check for broken links before committing

## Git workflow

- Never use `--no-verify` or skip pre-commit hooks
- Ask how to handle uncommitted changes before starting work
- Create a new branch when no clear branch exists for the changes
- Commit frequently throughout development
