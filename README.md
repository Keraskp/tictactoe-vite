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

### Components
Components in React always start with a Capital Letter. Component in React are functions which return JSX(JavaScript XML).
e.g A component named Square. 

Props are arguments passed into React components. Props are passed to components via HTML attributes. e.g value is passed in App.jsx which is received in Square.jsx
```javascript
const Square = ({ value }) => {
    console.log(value);
    return <div>Hello Square{value}</div>;
}

export default Square;
```

App.jsx
```javascript
import './App.css'
import Square from './components/Square.jsx';

function App() {
    return (
        <div className="card">
            <h1>Hello World</h1>
            <Square value="andrew"/>
        </div>
    );
}

export default App;
```

App.css contains css styling for the jsx.