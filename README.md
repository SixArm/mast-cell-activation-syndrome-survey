# Mast cell survey

```
mkdir mast-cell-survey && cd $_
npm create svelte@latest

npm install
git init && git add -A && git commit -m "Init"
npm run dev -- --open

git remote add origin git@github.com:SixArm/mast-cell-survey.git
git branch -M main
git push -u origin main
```


## CSS styles

Create file `src/app.css` with any global styles:

```css
h1 {
  color: red;
}
```

Note: using a separate CSS file is not required, but it is recommended, because it makes it easier for user interface designers to change the CSS.


## Layout

Create file `src/routes/+layout.svelte` with any layout that you want to use with all the routes:

```html
<script lang="ts">
  import './app.css';
  const { children } = $props()
</script>

{@render children()}
```

Note: the Svelte 5 syntax of "render children" replaces the deprecated Svelte 4 syntax of "slot".


# Default documentation

Everything you need to build a Svelte project, powered by [`create-svelte`](https://github.com/sveltejs/kit/tree/main/packages/create-svelte).

## Creating a project

If you're seeing this, you've probably already done this step. Congrats!

```bash
# create a new project in the current directory
npm create svelte@latest

# create a new project in my-app
npm create svelte@latest my-app
```

## Developing

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```bash
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

## Building

To create a production version of your app:

```bash
npm run build
```

You can preview the production build with `npm run preview`.

> To deploy your app, you may need to install an [adapter](https://kit.svelte.dev/docs/adapters) for your target environment.
