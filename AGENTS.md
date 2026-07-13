# AGENTS.md

This project is a one-page portfolio website for Prajit Narule, a short-form video editor. It was scaffolded from Netlify's TanStack Start portfolio template and then simplified into a focused client-facing landing page.

## Architecture

- `src/routes/__root.tsx` defines the root document and SEO metadata.
- `src/routes/index.tsx` contains the full portfolio page: hero, portfolio video grid, about, services, and contact sections.
- `src/styles.css` holds Tailwind imports, base theme tokens, global font smoothing, selection color, and page background defaults.
- `public/` stores static assets from the starter. The current homepage does not depend on custom local media assets.
- `netlify.toml`, `vite.config.ts`, and `package.json` provide the Netlify, Vite, TanStack Start, and Tailwind setup.

## Coding Conventions

- Keep the homepage as a single route unless a user explicitly asks for more pages.
- Use Tailwind utility classes for page styling and keep custom CSS limited to global defaults.
- Use the established green palette only for accents, links, buttons, borders, and highlights.
- Keep typography hierarchy simple: large bold headings and lighter, smaller body copy.
- Prefer lightweight static content and embedded media over client-side state or unnecessary animation.
- Use Lucide React icons when adding service or contact affordances.

## Non-Obvious Decisions

- The five portfolio videos are embedded directly in a responsive grid and are all visible in the portfolio section, matching the user's requirement to avoid hidden carousels.
- The design uses a dark neutral background with light green accents to stay professional while keeping the requested green-only color direction.
- Template routes and sample markdown content were removed so the deployed experience stays focused on the single portfolio page.
