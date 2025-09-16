# Repository Guidelines

## Project Structure & Module Organization
- Core documentation lives in `.mdx` files at the repo root and within topic folders like `concepts/`, `configuration/`, `cli/`, `api-reference/`, `guides/`, and `advanced/`.
- Global navigation, theming, and analytics reside in `mint.json`; update it whenever pages move and keep nav labels in sync with headings.
- Shared assets (images, logos) are stored alongside the docs they illustrate; prefer relative paths so Mintlify can bundle them correctly.

## Build, Test, and Development Commands
- `npm install` once to fetch dependencies for the Mintlify CLI if you prefer a local install.
- `npm run dev` (alias for `mint dev`) launches the hot-reloading docs server at `http://localhost:3000`.
- `npm run build` (`mint build`) performs a production build; use it to catch broken imports or MDX syntax errors before opening a PR.
- `npm run preview` opens the static build locally to sanity-check navigation and links.
- `npm run deploy` deploys through Mintlify; only run after the main branch is green.

## Coding Style & Naming Conventions
- Write documentation in clear, active voice and keep page titles sentence case to match existing navigation.
- Use MDX components from Mintlify (e.g., `<Tabs>`, `<Steps>`, `<Note>`) for structured guidance; prefer Markdown lists over HTML.
- Keep filenames kebab-case (e.g., `instant-features.mdx`) and align top-level `#` heading with the filename.
- Maintain concise front-matter metadata when needed and group related callouts together rather than scattering them.

## Testing Guidelines
- Treat `mint build` as the gatekeeper test; run it before commits to ensure MDX compiles and links resolve.
- For significant nav edits, open `mint preview` to manually verify sidebar ordering, cards, and cross-links.
- When adding interactive components, confirm they render without console warnings in the dev server.

## Commit & Pull Request Guidelines
- Follow the existing history: start commit subjects with a capitalized verb (e.g., “Refactor installation docs...”) and keep them specific.
- Reference affected sections or files in the body when changes span multiple pages; include rationale for structural shifts.
- Pull requests should summarize user-facing changes, list preview steps (`mint build` output), and link to Jira/GitHub issues when available. Attach screenshots for substantial visual updates.
