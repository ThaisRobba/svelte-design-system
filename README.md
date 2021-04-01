
# Svelte Design System

A very simple base for building a design system with Svelte.

Clone it with Git (or with degit, for actual use).

```bash
cd svelte-design-system
npm install # or yarn
```

## Gotchas

### Naming

Files with the `.wc.svelte` suffix will be built as web components, meaning that they *must* have an unique tag. View `src/theme-container.wc.svelte` for reference.

### Tags

Tags should have a small preffix, probably something related to the company developing the design system. In our case here, I used `pg` for `Pagar.me`. This is to avoid potential clashes with 3rd party libraries or even changes to the DOM spec

### Global styles

Global styles and web components don't mix too well. Ideally, you should use a themeing component to set CSS variables. View `src/theme-container.wc.svelte` and `src/body-text.wc.svelte` for reference.

### Exporting web components

They should be exported from the `src/index.js`. This ideally should be automated in larger projects (we don't even have a `npm serve` or anything like that here).

# Other References

https://javascript.plainenglish.io/can-you-build-web-components-with-svelte-3c8bc3c1cfd8

https://dev.to/silvio/how-to-create-a-web-components-in-svelte-2g4j

https://developers.google.com/web/fundamentals/web-components/best-practices