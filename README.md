# General Information

This project is powered by [`create-svelte`](https://github.com/sveltejs/kit/tree/master/packages/create-svelte).
It has been tweaked for fitting my own style/projects.
**This project has been configured to use typescript**

# Development tools
  
  TailwindCSS
  Playwright
  Vitest

## TailwindCSS

A utility-first CSS framework packed with classes like `flex, pt-4, text-center` that can be composed to build any design, directly in your markup.

### Examples

Tailwind can be used inline adding a class attribute to an HTML element
`class="text-center"`

It also can be used within the `style` block
```html
<button class="btn-primary">

<style lang="postcss">
  .btn-primary {
    @apply py-2 px-4 bg-blue-500 hover:bg-blue-700;
  }
</style>
```
**Important**
Do not use `@layer` in component styles aka inside `<style>` blocks.
Note how attribute `lang="postcss"` is used when tailwind `@apply` is being used.

## Playwright

Playwright enables reliable end-to-end testing for modern web apps.
**Important**
When running playwright for the first time it's most likely that the command `npx playwright install`
must be ran first to be able to run integration tests.

Integration tests are under `tests/integration` Folder.

To run integration tests run the following command: `npm run test:integration`

## Vitest

A Vite-native unit test framework.
Reuse Vite's config, transformers, resolvers, and plugins - consistent across your app and tests.

Jest Compatible
Expect, snapshot, coverage, and more.

ESM, TypeScript, JSX
Out-of-box ESM, TypeScript and JSX support powered by esbuild.

Unit tests are under `tests/unit`

To run unit tests run the following command: `npm run test:unit`

# Development

Once the project has been created and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server.

```bash
npm run dev

# If you want to add params run the following command
npm run dev -- {params}

# Params list
# --open : open the app in a new browser tab
# --host : exposes the app

```

# Build

To create a production version of your app:

```bash
npm run build
```

You can preview the production build with `npm run preview`.

# Deployment

To deploy your app, you may need to install an [adapter](https://kit.svelte.dev/docs/adapters) for your target environment.