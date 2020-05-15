# cra-template-reason-tailwind-ppx

This is a [ReasonML](https://reasonml.github.io/) + [ReasonReact](https://reasonml.github.io/reason-react/en/) template for [Create React App](https://github.com/facebook/create-react-app) featuring [TailwindCSS](https://tailwindcss.com) and [dylanirlbeck/tailwind-ppx](https://github.com/dylanirlbeck/tailwind-ppx) for type-safe `css`.

## Install

To use this template, add `--template @idkjs/reason-tailwind-ppx` when creating a new app.

For example:

```sh
npx create-react-app my-app --template @idkjs/reason-tailwind-ppx
# or
yarn create react-app my-app --template @idkjs/reason-tailwind-ppx
```

## Highlights

**Silences ESLint's Bucklescript Errors**

Available since [react-scripts@0.5.0](https://create-react-app.dev/docs/adding-custom-environment-variables#adding-development-environment-variables-in-env),
this template adds an `.eslintignore` file in the root directory with `*.bs.js` so that `react-scripts` ignores javascript errors which have already been handled by `bucklescript`. The `javascript` is 100% safe with [ReasonML](https://reasonml.github.io/) so we don't have to worry about these `eslint` warnings. To disable, remove `*.bs.js` from `.eslintignore` or remove `.eslintignore`. Remove `EXTEND_ESLINT=true` from you `.env` file.

**TailWind PPX**

See [bsconfig.json](template/bsconfig.json) for the default set up. Styles are set in [src/styles/tailwind.css](template/src/styles/tailwind.css) and [src/styles/index.css](template/src/styles/index.css) and compiled with the `build:styles` script in `package.json`.

## For more information, please refer to:

- [Getting Started](https://create-react-app.dev/docs/getting-started) – How to create a new app.
- [User Guide](https://create-react-app.dev) – How to develop apps bootstrapped with Create React App.
- [Building A Template](https://create-react-app.dev/docs/custom-templates/#building-a-template) – How to build a custom Create React App Template.
- [EXTEND_ESLINT=true](https://create-react-app.dev/docs/advanced-configuration) - Define permanent environment variables in a creat-react-app project.
- [Tailwind-PPX](https://github.com/dylanirlbeck/tailwind-ppx) - Reason/OCaml PPX for writing compile-time validated Tailwind CSS classes.
- [TailwindCSS](https://tailwindcss.com) - A utility-first CSS framework for
rapidly building custom designs.