# kubetail-ui

Kubetail-UI is a project for developing and sharing React components and other UI elements for Kubetail

## Getting started

First, install the dependencies:

```sh
pnpm install
```

Next, run storybook:

```sh
pnpm storybook
```

Open [http://localhost:6006](http://localhost:6006) in your browser to see the components.

## Scripts

* build - Run the build script (`$ pnpm build`)
* lint - Run the linter (`$ pnpm lint`)
* test - Run the unit tests (`$ pnpm test`)
* storybook - Run the storybook development server (`$ pnpm storybook`)
* build-storybook - Run the storybook build script (`$ pnpm build-storybook`)

## Integrate kubetail-ui into your Tailwind CSS project

1. Install `kubetail-ui` package (replace X.Y.Z with desired version)

```bash
pnpm add git+ssh://git@github.com/kubetail-org/kubetail-ui.git#vX.Y.Z
```

2. Modify your Tailwind config file

```javascript
module.exports = {
  content: [
    ...
    "./node_modules/kubetail-ui/esm/*.js"
  ],
  plugins: [
    ...
    require('kubetail-ui/plugin')
  ]
}
```
