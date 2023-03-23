#Tips prueba tecnicas React

-Instalacion de react desde cero con Vite (Abrir terminal)

````
```
npm install @vitejs/plugin-react -E
//Escoger Vanilla y Javascript

npm install react react-dom -E

```
````

-Creacion del fichero vite.config.js

````
```
import { defineConfig } from "vite";
import react from '@vitejs/plugin-react'

 export default defineConfig({ 
    plugins: [ react() ] 
})
```
````

- Renombrar archivo main.js a main.jsx

````
```
<div id="app"></div>
<script type="module" src="/main.jsx"></script>
```
````

- Eliminar contenido del main.jsx y crear manualmente

````
```
import { createRoot } from 'react-dom/client'

const root = createRoot( document.getElementById('app'));
root.render(
    <h1> Hello World</h1>
    /*O algun componente normal de react*/
)

```
````

- Importante: instalar ESLINT
````
```
npm install standard -D

/*Ir al package.json*/

"eslintConfig":{
   "extends": "./node_modules/standard/eslintrc.json"
}
```
````
