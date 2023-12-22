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

## Astro References

### Create and deploy your first Astro Site

[FreeCodeCamp.org](https://freecodecamp.org/)

[Using Git Source control in VS Code](https://code.visualstudio.com/docs/sourcecontrol/overview#_git-support)

[A step-by-step guide to deploying on Netify](https://www.netlify.com/blog/2016/09/29/a-step-by-step-guide-deploying-on-netlify/)

### Unit 2: Pages

- Create your first Astro pages with the .astro syntax
- Add blog posts with Markdown (.md) files
- Style an individual page with `<style>`
- Apply global styles across pages

#### [Create your first Astro page](https://docs.astro.build/en/tutorial/2-pages/1/)

- Create a new .astro file
- Edit your page
- Add navigation links
- Try it yourself
- Add a Blog page
- Publish your changes to the web

[File-based Routine in Astro](https://docs.astro.build/en/core-concepts/astro-pages/#file-based-routing)

[Astro Page HTML](https://docs.astro.build/en/core-concepts/astro-pages/#astro-pages)

#### [Write your first Markdown Blog Post](https://docs.astro.build/en/tutorial/2-pages/2/)

- Create your first .md file
- Write Markdown content
- Link to your posts

[Markdown Cheat Sheet from The Markdown Guide](https://www.markdownguide.org/cheat-sheet/)

[Fire Fox Devtools Docs](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/What_are_browser_developer_tools)

[YAML Frontmatter](https://assemble.io/docs/YAML-front-matter.html)

#### [Add dynamic content about you](https://docs.astro.build/en/tutorial/2-pages/3/)

- Define and use a variable
- Write JavaScript expressions in Astro
- Conditionally render elements

[Dynamic Expressions in Astro](https://docs.astro.build/en/core-concepts/astro-syntax/#jsx-like-expressions)

#### [Style your about page](https://docs.astro.build/en/tutorial/2-pages/4/)

- Style an individual page
- Use your first CSS variable
- Try it yourself - Define CSS variables

[Astro syntax vs JSX - comparision](https://docs.astro.build/en/core-concepts/astro-syntax/#differences-between-astro-and-jsx)

[Astro `<style>` tag](https://docs.astro.build/en/guides/styling/#styling-in-astro)

[CSS variables in Astro](https://docs.astro.build/en/guides/styling/#css-variables)

#### [Add site-wide styling](https://docs.astro.build/en/tutorial/2-pages/5/)

### Unit 3: Components

- A Navigation component that presents a menu of links to your pages
- A Footer component to include at the bottom of each page
- A Social Media component, used in the Footer, that links to profile pages
- An interactive Hamburger component to toggle the Navigation on mobile

#### [Make a reusable Navigation component](https://docs.astro.build/en/tutorial/3-components/1/)

- Create a new src/components/ folder
- Create a Navigation component

[Astro Component Overview](https://docs.astro.build/en/core-concepts/astro-components/)

[Refactoring](https://refactoring.com/)

#### [Create a social media footer](https://docs.astro.build/en/tutorial/3-components/2/)

- Create a Footer Component
- Try it yourself - Personalize your footer
- Create a Social Media component
- Style your Social Media Component

[Component Props in Astro](https://docs.astro.build/en/core-concepts/astro-components/#component-props)

#### [Build it yourself - Header](https://docs.astro.build/en/tutorial/3-components/3/)

- Try it yourself - Build a new Header component
- Try it yourself - Update your pages
- Add responsive styles

[Component-based Design](https://www.droptica.com/blog/component-based-design/)

[Semantic HTML Tags](https://www.dofactory.com/html/semantics)

[Mobile-first Design](https://www.mobileapps.com/blog/mobile-first-design)

#### [Send your first script to the browser](https://docs.astro.build/en/tutorial/3-components/4/)

- Build a Hamburger component
- Write your first script tag

[Client-side scripts in Astro](https://docs.astro.build/en/guides/client-side-scripts/)

### Unit 4 Layouts

- Create reusable layout components
- Pass content to your layouts with <slot />
- Pass data from Markdown frontmatter to your layouts
- Nest multiple layouts

#### [Build your first layout](https://docs.astro.build/en/tutorial/4-layouts/1/)

- Create your first layout component
- Use your layout on a page
- Pass page-specific values as props
- Try it yourself - Use your layout everywhere

[Astro layout components](https://docs.astro.build/en/core-concepts/layouts/)

[Astro `<slot />`](https://docs.astro.build/en/core-concepts/astro-components/#slots)

#### [Create and pass data to a custom blog layout](https://docs.astro.build/en/tutorial/4-layouts/2/)

- Add a layout to your blog posts
- Try it yourself - Customize your blog post layout

[Markdown Layouts in Astro](https://docs.astro.build/en/guides/markdown-content/#frontmatter-layout)

[Markdown Layout Props](https://docs.astro.build/en/core-concepts/layouts/#markdown-layout-props)

[Introduction to YAML](https://dev.to/paulasantamaria/introduction-to-yaml-125f)

#### [Combine layouts to get the best of both worlds](https://docs.astro.build/en/tutorial/4-layouts/3/)

- Nest your two layouts

[Nesting Layouts in Astro](https://docs.astro.build/en/core-concepts/layouts/#nesting-layouts)

### Unit 5 - Astro API

- Astro.glob() to access data from files in your project
- getStaticPaths() to create multiple pages (routes) at once
- The Astro RSS package to create an RSS feed

#### [Create a blog post archive](https://docs.astro.build/en/tutorial/5-astro-api/1/)

- Dynamically display a list of posts
- Challenge: Create a BlogPost component

[`Astro.glob()` API Documentation](https://docs.astro.build/en/reference/api-reference/#astroglob)

#### [Generate tag pages](https://docs.astro.build/en/tutorial/5-astro-api/2/)

- Dynamic page routing
- Create pages dynamically
- Use props in dynamic routes
- Advanced JavaScript: Generate pages from existing tags

[Dynamic Page Routine in Astro](https://docs.astro.build/en/core-concepts/routing/#dynamic-routes)

[`getStaticPaths()` API Documentaiton](https://docs.astro.build/en/reference/api-reference/#getstaticpaths)

#### [Build a tag index page](https://docs.astro.build/en/tutorial/5-astro-api/3/)

- Use the /pages/folder/index.astro routing pattern
- Try it yourself - Make a Tag Index page
- Create an array of tags
- Create your list of tags
- Add styles to your tag list
- Add this page to your navigation
- Challenge: Include tags in your blog post layout

[Static Routing in Astro](https://docs.astro.build/en/core-concepts/routing/#static-routes)

#### [Add an RSS feed](https://docs.astro.build/en/tutorial/5-astro-api/4/)

- Install Astro’s RSS package
- Create an .xml feed document

[RSS item generation in Astro](https://docs.astro.build/en/guides/rss/#using-glob-imports)

### Unit 6 - Astro Islands

- Add a UI framework, Preact, to your Astro project
- Use Preact to create an interactive greeting component
- Learn when you might not choose islands for interactivity

#### [Build your first Astro island](https://docs.astro.build/en/tutorial/6-islands/1/)

- Add Preact to your Astro project
- Include a Preact greeting banner

[Astro Integrations Guide](https://docs.astro.build/en/guides/integrations-guide/)

[Using UI Framework Components in Astro](https://docs.astro.build/en/core-concepts/framework-components/#using-framework-components)

[Astro client directives reference](https://docs.astro.build/en/reference/directives-reference/#client-directives)

#### [Back on dry land. Take your blog from day to night, no island required!]

- Add and style a theme toggle icon
- Add CSS styling for a dark theme
- Add client-side interactivity

[Client-side '<scripts>' in Astro](https://docs.astro.build/en/guides/client-side-scripts/)
