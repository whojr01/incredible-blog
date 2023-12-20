# Astro tutorial

Following the Astro Blog tutorial located at [Blog](https://docs.astro.build/en/tutorial/1-setup/2/)

## setup

npm install astro@latest

When the prompt asks, “Would you like to install dependencies?” type y.

When the prompt asks you if you plan on writing TypeScript, type n.

When the prompt asks, “Would you like to initialize a new git repository?” type y.

## Run astro server

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

## Documentation 👀

[our documentation](https://docs.astro.build)

## Git Repository

…or create a new repository on the command line
`echo "# incredible-blog" >> README.md`
`git init`
`git add README.md`
`git commit -m "first commit"`
`git branch -M main`
`git remote add origin https://github.com/whojr01/incredible-blog.git`
`git push -u origin main`

…or push an existing repository from the command line
`git remote add origin https://github.com/whojr01/incredible-blog.git`
`git branch -M main`
`git push -u origin main`

## Deploying to Netify

Site URL: whojr.netify.app

## Adding pages

[Astro Pages](https://docs.astro.build/en/core-concepts/astro-pages/#astro-pages)

Astro leverages a routing strategy called file-based routing. Each file in your `src/pages/` directory becomes an endpoint on your site based on its file path.

Link between pagesSection titled Link between pages
Write standard HTML <a> elements in your Astro pages to link to other pages on your site. Use a URL path relative to your root domain as your link, not a relative file path.

For example, to link to https://example.com/authors/sonali/ from any other page on example.com:

Read more <a href="/authors/sonali/">about Sonali</a>.

Partials are page components located within src/pages/ that are not intended to render as full pages.

Like components located outside of this folder, these files do not automatically include the <!DOCTYPE html> declaration, nor any <head> content such as scoped styles and scripts.

## Astro routing

[Astro Routing](https://docs.astro.build/en/core-concepts/astro-pages/#file-based-routing)

## Markdown Cheat Sheet

[Markdown Cheat Sheet from The Markdown Guide](https://www.markdownguide.org/cheat-sheet/)

## Firefox Devtool docs

[Fire Fox Devtools Docs](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/What_are_browser_developer_tools)

## YAML Frontmatter

[YAML Frontmatter](https://assemble.io/docs/YAML-front-matter.html)
