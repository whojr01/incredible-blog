# [Tutorial - Extend with Content Collections](https://docs.astro.build/en/tutorials/add-content-collections/)

Content collections are a powerful way to manage groups of similar content, such as blog posts. Collections help to organize your documents, validate your YAML frontmatter, and provide automatic TypeScript type-safety for all of your content (even if you don’t write any TypeScript yourself).

- Move your folder of blog posts into src/content/
- Create a schema to define your blog post frontmatter
- Use getCollection() to get blog post content and metadata

## Pages vs Collections

Even when using content collections, you will still use the src/pages/ folder for individual pages, such as your About Me page. But, moving your blog posts to the special src/content/ folder will allow you to use more powerful and performant APIs to generate your blog post index and display your individual blog posts.

[Astro's content collections](https://docs.astro.build/en/guides/content-collections/)

## Setup typescript

- Blog tutorial used `base` least strict
- Content tutorial uses either `strict` or `strictness`

In order to use content collections without writing TypeScript in the rest of the blog tutorial example, add the following two TypeScript configuration options to the config file:

tscongif.json

```
{
  // Note: No change needed if you use "astro/tsconfigs/strict" or "astro/tsconfigs/strictest"
  "extends": "astro/tsconfigs/base",
  "compilerOptions": {
    "strictNullChecks": true,
    "allowJs": true
  }
}
```

## [Create Collection](https://docs.astro.build/en/tutorials/add-content-collections/#extending-the-blog-tutorial-with-content-collections)

Collecitons are defined in `/src/content/{Colleciton type}` where colleciton type could be `posts`, `authors`, `profiles`...etc.

### [Defining Collection Schema](https://docs.astro.build/en/guides/content-collections/#defining-a-collection-schema)

The collection schema file `/src/content/config.ts` contains all collection schema's.

## [Querying your collection](https://docs.astro.build/en/guides/content-collections/#querying-collections)

This makes the blog post's slug and page content available to each page it will generate.

```
---
import { getCollection } from 'astro:content';
export async function getStaticPaths() {
  const blogEntries = await getCollection('posts');
  return blogEntries.map(entry => ({
    params: { slug: entry.slug }, props: { entry },
  }));
}

const { entry } = Astro.props;
const { Content } = await entry.render();
---

<MarkdownPostLayout frontmatter={entry.data}>
  <Content />
</MarkdownPostLayout>

```
