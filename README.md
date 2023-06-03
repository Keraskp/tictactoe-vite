# Vite
Vite uses rollup under the hood.

`index.html` is the entry point of the project. It sources the script to the react app which is present inside `./src`
`./public` contains all the static assets to be rendered.

`.eslintrc`, `.prettierrc` are part of project configuration

Runs local development server for the Vite project
```
npm run dev
```

Creates a `./dist` directory which contains svg, html, css and js files. These files are built from the `./src` directory.
```
npm run build
```

git ignores `/dist` and `/node_modules` because these are dynamically generated in the server.
```
npm install
npm run build
```
