# Laura Sofía Gómez Rosales — Portfolio

Personal portfolio and CV website for **Laura Sofía Gómez Rosales**, Systems Engineer and Master's student in Cloud Computing & Infrastructure (MoSIG) at Grenoble INP – Ensimag.

## Live site

[https://slrosales.github.io](https://slrosales.github.io)

## Tech stack

- [Astro](https://astro.build)
- [TailwindCSS](https://tailwindcss.com/)
- [DaisyUI](https://daisyui.com/)

## Getting started

```bash
pnpm install
pnpm run dev
```

Build the production site:

```bash
pnpm run build
```

## Project structure

```php
src/
├── components/   # Reusable UI (cards, sidebar, header, footer, timeline)
├── content/      # Markdown content collections (blog, store)
├── layouts/      # BaseLayout, PostLayout, StoreItemLayout
├── pages/        # Routes (index, projects, research, cv, blog, store)
└── config.ts     # Global site config (name, title, description, bio, location)
```

## Customization

Global site settings live in [`src/config.ts`](src/config.ts) — name, site title, description, bio, and location.

- **Homepage** — [`src/pages/index.astro`](src/pages/index.astro)
- **Projects** — [`src/pages/projects.astro`](src/pages/projects.astro)
- **CV / Resume** — [`src/pages/cv.astro`](src/pages/cv.astro)
- **Research & Publications** — [`src/pages/research.astro`](src/pages/research.astro)
- **Blog posts** — add Markdown files to `src/content/blog/`

The theme can be changed via the `data-theme` attribute in [`src/layouts/BaseLayout.astro`](src/layouts/BaseLayout.astro) (see [DaisyUI themes](https://daisyui.com/docs/themes/)).

## Deployment

Deployed as a static site on [GitHub Pages](https://pages.github.com/). Sitemap and RSS feed are generated automatically on build. See the [Astro deployment guide](https://docs.astro.build/en/guides/deploy/) for other platforms.

## Credits

Built on top of [Astrofy](https://github.com/manuelernestog/astrofy), a free and open-source portfolio template created by [Manuel Ernesto](https://github.com/manuelernestog).

## License

[MIT](LICENSE)
