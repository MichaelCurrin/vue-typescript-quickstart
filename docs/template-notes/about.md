# About

## Resources

- [Vue 3 homepage](https://v3.vuejs.org/)
- [Vue Installation](https://v3.vuejs.org/guide/installation.html)
- [TypeScript Support](https://v3.vuejs.org/guide/typescript-support.html) - this explains how to configure your project and how to add TypeScript to your Vue components.
- [Class components](https://class-component.vuejs.org/)


## Add TypeScript

For an existing Vue project, you can the TypeScript plugin

```sh
$ vue add typescript
...
✔  Successfully installed plugin: @vue/cli-plugin-typescript
```


## Create a new project from scratch

This project was generated using the Vue CLI. You can follow these steps below.

Optionally install Vue CLI globally:

```sh
$ npm install -g @vue/cli
```

Create a new project - you can run this even if you don't have Vue installed.

```sh
$ npx vue create my-project-name
```

When I ran that, here are options I saw and chose to make this template project.

- Packages - I only added TypeScript.
    ```
    ❯◉ Babel
    ◉ TypeScript
    ◯ Progressive Web App (PWA) Support
    ◯ Router
    ◯ Vuex
    ◯ CSS Pre-processors
    ◉ Linter / Formatter
    ◯ Unit Testing
    ◯ E2E Testing
    ```
- Vue: 3
- Babel: Yes
    > Use Babel alongside TypeScript (required for modern mode, auto-detected polyfills, transpiling JS
- Class components: No
- Linter / formatter:
    The first was the default but I like Prettier so chose that.
    ```
    ESLint with error prevention only
    ESLint + Airbnb config
    ESLint + Standard config
    ❯ ESLint + Prettier
    TSLint (deprecated)
    ```
- Additional lint features:
    ```
    ❯◉ Lint on save
    ◯ Lint and fix on commit
    ```
- Where do you prefer placing config for Babel, ESLint, etc.? (Use arrow keys)
    ```
    ❯ In dedicated config files
    In package.json
    ```

The tool sets up a project that uses Yarn.
