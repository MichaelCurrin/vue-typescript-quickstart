# Development


## Errors

See [shims-vue.d.ts](/src/shims-vue.d.ts).

The file causes two warnings when used with Prettier and ESLint.

These files were created to deal with that:

- [.prettierignore](/.prettierignore)
- [.eslintignore](/.estlintignore)

### Prettier error

This looks like a TS compatibility issue in Prettier. It is closed but I still see the issue in latest versions of Prettier, TS and ESLint plugins.

https://github.com/prettier/prettier/issues/7263

```
warning: Parsing error: '=' expected (prettier/prettier) at src/shims-vue.d.ts:2:16:
  1 | declare module '*.vue' {
> 2 |   import type { DefineComponent } from 'vue'
    |                ^
  3 |   const component: DefineComponent<{}, {}, any>
  4 |   export default component
  5 | }
```

The inline use of `// prettier-ignore` did not work.

### Linting types error

The use of `{}` and `any` should just be ignored as I don't know enough about these tools to put in a better replacement.

```
error: Don't use `{}` as a type. `{}` actually means "any non-nullish value".
- If you want a type meaning "any object", you probably want `Record<string, unknown>` instead.
- If you want a type meaning "any value", you probably want `unknown` instead.
- If you want a type meaning "empty object", you probably want `Record<string, never>` instead (@typescript-eslint/ban-types) at src/shims-vue.d.ts:3:40:
  1 | declare module '*.vue' {
  2 |   import type { DefineComponent } from 'vue'
> 3 |   const component: DefineComponent<{}, {}, any>
    |                                        ^
  4 |   export default component
  5 | }
  6 |
```

And also:

```
warning: Unexpected any. Specify a different type (@typescript-eslint/no-explicit-any) at src/shims-vue.d.ts:3:44:
  1 | declare module '*.vue' {
  2 |   import type { DefineComponent } from 'vue'
> 3 |   const component: DefineComponent<{}, {}, any>
    |                                            ^
  4 |   export default component
  5 | }
```
