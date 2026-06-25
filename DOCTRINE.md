# DOCTRINE.md - mintlify-docs

**Status:** v0.1
**Steward:** HUMMBL Research Institute

## 1. Thesis
This repo hosts HUMMBL's public-facing documentation deployed via Mintlify. The bet is that a dedicated docs deployment — with structured navigation, API references, and component-based pages — provides better developer experience than scattered READMEs across the fleet.

The repo is a Mintlify configuration surface: docs.json defines navigation and branding, page content lives in Markdown, and changes propagate to production automatically on push to the default branch.

## 2. Conceptual vocabulary
- **docs.json** — Mintlify configuration file defining navigation, branding, and page structure.
- **Mintlify CLI** — local development server (`mint dev`) for previewing documentation changes.
- **Page** — Markdown file rendered with Mintlify components and navigation.
- **Deployment** — automatic propagation from default branch push to production.

## 3. Design principles
1. Docs are a product surface — treat them with the same rigor as code.
2. Preview before publish — use `mint dev` locally before pushing changes.
3. Navigation is UX — structure docs.json for the reader's journey, not the writer's convenience.
4. Keep pages focused — one concept per page; link rather than inline.

## 4. Boundaries
- Not a code repository — documentation content only.
- Not a governance artifact store — those live in their respective repos.
- Not a replacement for inline READMEs — this is the public-facing summary surface.

## 5. Open questions
- Should docs auto-generate from repo READMEs or remain hand-curated?
- How to version documentation across HUMMBL framework releases?
- What is the review process for docs changes — same as code PRs or lighter?
