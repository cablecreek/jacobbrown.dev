# JB's personal site and blog

## post deployment checks:
1. Lighthouse 
2. PageSpeed
    - https://pagespeed.web.dev/
3. Rich Results
    - https://search.google.com/test/rich-results
4. https://jacobbrown.dev/static/robots.txt
5. https://jacobbrown.dev/static/sitemap.xml 
6. https://www.opengraph.xyz/
7. https://metatags.io/
8. Google Search Console 
    1. Check Coverage (indexing status).
    2. Check Enhancements (schema, breadcrumbs, mobile usability).
    3. Check Core Web Vitals.
    4. Submit sitemap (once, unless it changes structure).
    5. Request Reindex only when important changes happen.
        - paste in top bar
        - test live site
        - then request 

- Test social previews 
    - MetaTags.io 
    - OpenGraph.xyz  
    - Twitter Validator.

## SEO
check seo and index site
- https://metatags.io/
- google search console
- google analytics

### Essential
- Title
- Meta Description
- Viewport (auto set by nextjs)
- Canonical Tag
- author
- sitemap.xml
- manifest.json
- robots.txt

### Optional (but recommended) 
- Open Graph
- Twitter Cards
- favicon, icon, and apple-icon
- keywords
## Project Structure 
- this is based on the Astro starter blog.
- see the following folders and files:

```text
├── public/
├── src/
│   ├── components/
│   ├── content/
│   ├── layouts/
│   └── pages/
├── astro.config.mjs
├── README.md
├── package.json
└── tsconfig.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

There's nothing special about `src/components/`, but that's where we like to put any Astro/React/Vue/Svelte/Preact components.

The `src/content/` directory contains "collections" of related Markdown and MDX documents. Use `getCollection()` to retrieve posts from `src/content/blog/`, and type-check your frontmatter using an optional schema. See [Astro's Content Collections docs](https://docs.astro.build/en/guides/content-collections/) to learn more.

Any static assets, like images, can be placed in the `public/` directory.

## Commands


| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `pnpm install`             | Installs dependencies                            |
| `pnpm dev`             | Starts local dev server at `localhost:4321`      |
| `pnpm build`           | Build your production site to `./dist/`          |
| `pnpm preview`         | Preview your build locally, before deploying     |

