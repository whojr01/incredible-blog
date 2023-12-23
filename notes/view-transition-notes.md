# View Transitions

View transitions are added to the head element in the document. Not the header component but the head.

Then simply add the `<ViewTransitions />` tag before the head close.

## Update scripts

After a transition runs some scripts may no longer re-run after page navigation like they do with full browser refreshes.

## [Astro Events](https://docs.astro.build/en/guides/view-transitions/#lifecycle-events)

Use the astro events:

- `astro:before-preparation`
  - An event that fires at the beginning of the preparation phase, after navigation has started (e.g. after the user has clicked a link), but before content is loaded.
- `astro:after-preparation`
  - An event that fires at the end of the preparation phase, after the new page’s content has been loaded and parsed into a document. This event occurs before the view transitions phase.
- `astro:before-swap`
  - An event that fires before the new document (which is populated during the preparation phase) replaces the current document. This event occurs inside of the view transition, where the user is still seeing a snapshot of the old page.
- `astro:after-swap`
  - An event that fires immediately after the new page replaces the old page. You can listen to this event on the document and trigger actions that will occur before the new page’s DOM elements render and scripts run.
- `astro:page-load`
  - An event that fires at the end of page navigation, after the new page is visible to the user and blocking styles and scripts are loaded. You can listen to this event on the document.

`before` events allow you to influence and modify actions that are about to take place.
`after` events are notifications that a phase is complete.

## Customizing Transitions

With view transitions enabled, you currently have a small fade in and out set for all page transition animations. Astro also provides a built-in `slide` animation. To change the type of animation for a single element, add the `transition:animate=""` directive.

```
  <h1 transition:animate="slide">{pageTitle}</h1>
```

## [Transition directives](https://docs.astro.build/en/guides/view-transitions/#transition-directives)

```
  <p transition:animate={fade({ duration: '2s'})}><em>{frontmatter.description}</em></p>
```

## Force a full browser reload for some linksSection titled Force a full browser reload for some links

To make it so that your browser refreshes every time you click the navigation link to go to your About page, add the data-astro-reload attribute to the `<a>` tag in your `<Navigation />` component. This will override the `<ViewTransitions />` router entirely, and any of the view transition animations, for this one link.

```
  <a href="/about/" data-astro-reload>About</a>
```
