# DiopScan

CPSC 481- A machine learning application designed to analyze medical images and
detect potential signs of cancer

# Notebooks

## Run notebooks

```
uv sync
uv run --with jupyter jupyter lab notebooks/preprocess.ipynb
```


# Frontend

## Developing

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```sh
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

## Building

To create a production version of your app:

```sh
npm run build
```