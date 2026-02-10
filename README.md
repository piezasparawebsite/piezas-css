# css

En este repositorio, tenemos una serie de 
selectores (piezas) conocidos como class 
en css.

## como ?

Para utilizarlos es muy sencillo
unicamente agregas el selector 
al elemento.

### ejemplo

Si queremos generar una linea dorada
con gradiente y una longitud de 94px
tan sencillo como :

`<div class="linea-dorada"></div>`

### resultado:

![linea-dorada](linea-dorada.png)

## Recuerda

Para que esa clase (class|selector) funcione
debes de agregar el archivo linea-dorada.css
en el head del documento con la etiqueta `link`

Los archivos colores.css y cuerpo.css
son los estilos base para iniciar cualquier 
proyecto web.(los estilos).

En tu documento deben de estar ubicados
estos dos archivos de la siguiente manera:

```
<html>
    <head>
        <link rel="stylesheet" href="colores.css">
        <link rel="stylesheet" href="cuerpo.css">
    </head>
    <body>
    </body>
</html>
```

## pieza-paleta de colores

```css
:root {
    --bg-dark: #020617;
    --glass-bg: rgba(15, 23, 42, 0.8);
    --gold: #d4af37;
    --gold-bright: #f9e076;
    --gold-dark: #b8860b;
    --slate-300: #cbd5e1;
    --slate-500: #64748b;
    --slate-600: #475569;
    --slate-900: #0f172a;
    --green: #10b981;
    --red: #ef4444;
    --white: #ffffff;
}
```

## pieza-estado inicial del body

```css
* { margin: 0; padding: 0; box-sizing: border-box; }

body {
    background-color: var(--bg-dark);
    color: var(--slate-300);
    font-family: 'Inter', sans-serif;
    min-height: 100vh;
    line-height: 1.5;
}
```

el codigo anterior le da al body 
(el contenedor del contenido de tu pagina),
un color de fondo, color de fuente(letra),
una tipografia (font-family) , una altura inicial
(100vh) y un interlineado de 1.5

puedes cambiar el color inicial , colocando
el nombre de la variable definida en :root
dentro de la funcion var();