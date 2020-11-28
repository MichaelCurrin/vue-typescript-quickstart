# About

## Resources

- [Vue 3 homepage](https://v3.vuejs.org/)
- [Vue Installation](https://v3.vuejs.org/guide/installation.html)
- [TypeScript Support](https://v3.vuejs.org/guide/typescript-support.html)


## Create a new project from scratch

This project was generated using the Vue CLI. You can follow these steps below.

Optionally install Vue CLI globally:

```sh
$ npm install -g @vue/cli
```

Create the project. You can run this even if you don't have Vue installed.

```sh
$ npx vue create my-project-name
```

Then options were selected:

- Packages: (I added TypeScript)
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
