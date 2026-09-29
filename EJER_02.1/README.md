# React + Vite

## Ejercicio 1 · Explora la estructura del proyecto

### 1. ¿En qué archivo está el punto de entrada de la aplicación? ¿Qué hace la función createRoot?
El punto de entrada de la aplicación está en src/main.jsx. La función createRoot crea la raíz de React sobre el elemento HTML con id="root" y permite renderizar la aplicación React dentro de él.

### 2. ¿Cuál es el ID del elemento HTML donde se monta la aplicación? ¿En qué archivo está definido?
La aplicación se monta en el elemento `<div id="root">`, que está definido en `index.html`.

### 3. Dibuja el árbol de componentes que se renderiza al arrancar el proyecto recién creado.
root
└── StrictMode
    └── App

### 4. ¿Qué ocurre en la página si eliminas `<StrictMode>` de `main.jsx`? ¿Y en la consola en modo desarrollo?
Si elimino `<StrictMode>`, la página sigue funcionando igual. En desarrollo, algunas funciones que podían ejecutarse dos veces dejan de hacerlo y aparecen menos avisos en la consola.

### 5. Abre `App.jsx` y localiza tres fragmentos de código JavaScript escritos entre llaves `{ }` dentro del JSX. Explica qué hace cada uno.
- `{count}` muestra el valor actual del contador.
- `{() => setCount((count) => count + 1)}` aumenta el contador en 1 al pulsar el botón.
- `{heroImg}` utiliza la imagen guardada en la variable `heroImg`.

### 6. ¿Qué es el elemento `<>` que envuelve el JSX devuelto por `App`? ¿Genera algún elemento en el DOM? Compruébalo con las herramientas de desarrollo del navegador (pestaña *Elementos*).
`<>...</>` es un Fragment de React que permite agrupar varios elementos sin crear un elemento HTML adicional. Por eso no aparece como una etiqueta en el DOM al comprobarlo con las herramientas de desarrollo.