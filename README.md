# pokedex

[![pokedex](https://github.com/tcreator-proj/pokedex/actions/workflows/web.yml/badge.svg)](https://github.com/tcreator-proj/pokedex/actions/workflows/web.yml)

This template should help get you started developing with Vue 3 in Vite.

## Recommended IDE Setup

[VSCode](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur).

## Type Support for `.vue` Imports in TS

TypeScript cannot handle type information for `.vue` imports by default, so we replace the `tsc` CLI with `vue-tsc` for type checking. In editors, we need [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) to make the TypeScript language service aware of `.vue` types.

## Customize configuration

See [Vite Configuration Reference](https://vitejs.dev/config/).

## Project Setup

```sh
npm install
```

### Compile and Hot-Reload for Development

```sh
npm run dev
```

### Type-Check, Compile and Minify for Production

```sh
npm run build
```

### Run Unit Tests with [Vitest](https://vitest.dev/)

```sh
npm run test:unit
```

### Run End-to-End Tests with [Playwright](https://playwright.dev)

##### unix
```bash
sudo docker run --rm --network host -v $(pwd)/:/work/ -w /work/ -it mcr.microsoft.com/playwright:v1.44.1-jammy /bin/bash
```

```shell
docker run --rm --network host -v ${pwd}/:/work/ -w /work/ -it mcr.microsoft.com/playwright:v1.44.1-jammy /bin/bash
```

```bash
apt update \
&& apt install build-essential -y --no-install-recommends \
&& yarn \
&& yarn build \
&& xvfb-run yarn test:playwright 
```
### Lint with [ESLint](https://eslint.org/)

```sh
npm run lint
```
