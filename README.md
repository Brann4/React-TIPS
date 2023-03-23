# Tips prueba tecnicas React

## 1. Instalacion de react desde cero con Vite (Abrir terminal)

````
npm install @vitejs/plugin-react -E
//Escoger Vanilla y Javascript

npm install react react-dom -E

````

## 2.Creacion del fichero vite.config.js

````
```javascript
import { defineConfig } from "vite";
import react from '@vitejs/plugin-react'

 export default defineConfig({ 
    plugins: [ react() ] 
})
```
````

## 3.Renombrar archivo main.js a main.jsx

````
<div id="app"></div>
<script type="module" src="/main.jsx"></script>
````

## 4.Eliminar contenido del main.jsx y crear manualmente

````
```javascript
import { createRoot } from 'react-dom/client'

const root = createRoot( document.getElementById('app'));
root.render(
    <h1> Hello World</h1>
    /*O algun componente normal de react*/
)

```
````

## 5.Importante: instalar ESLINT
````
npm install standard -D
````

````
```javascript
"eslintConfig":{
   "extends": "./node_modules/standard/eslintrc.json"
}
```
````
