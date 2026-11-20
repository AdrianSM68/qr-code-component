# QR Code Component

Componente de tarjeta con un código QR, desarrollado como práctica de maquetación a partir del reto **QR Code Component** de Frontend Mentor.

El objetivo del proyecto es reproducir una interfaz sencilla y limpia utilizando HTML, CSS y el preprocesador LESS. Los colores se tomaron de la imagen de referencia mediante la herramienta **PicPick**.

## Vista del componente

El diseño consta de una tarjeta blanca sobre un fondo azul grisáceo, con una imagen QR, un título y una breve descripción.

![Imagen del código QR](img/image-qr-code.png)

## Tecnologías utilizadas

- **HTML5** para la estructura y el contenido.
- **CSS3** para los estilos, la tipografía, los espaciados y los bordes redondeados.
- **LESS** para organizar los estilos mediante variables y selectores anidados.
- **Outfit** como tipografía, cargada desde un archivo local de fuente variable.

No se utiliza JavaScript.

## Estructura del proyecto

La estructura que espera el HTML y las rutas relativas de los estilos es la siguiente:

```text
proyecto/
├── index.html
├── css/
│   ├── styles.less
│   └── styles.css
└── img/
    ├── image-qr-code.png
    ├── favicon-32x32.png
    └── fonts/
        └── Outfit-VariableFont_wght.ttf
```

> Los archivos de estilos adjuntos pueden tener otros nombres. Para ejecutar esta estructura, hay que guardarlos como `styles.less` y `styles.css` dentro de `css/`, según la ruta enlazada en el HTML.

## Cómo ejecutar el proyecto

1. Coloca los archivos en las rutas indicadas en la estructura anterior.
2. Si has modificado el LESS, compílalo a CSS (por ejemplo, con `npx lessc css/styles.less css/styles.css`, teniendo disponible el compilador LESS).
3. Abre `index.html` en el navegador.

Para visualizar la página **no necesitas JavaScript ni un servidor**; basta con disponer del CSS compilado y los recursos locales.

## Detalles del diseño

- Tarjeta de **320 px** de ancho, con fondo blanco y esquinas de **20 px**.
- Imagen QR de **290 px** de ancho, con esquinas de **10 px**.
- Título de **21 px** y descripción de **14 px**.
- Contenido alineado al centro y una sombra sutil bajo la tarjeta.
- Colores obtenidos con **PicPick** y centralizados parcialmente en variables LESS.

Consulta [`style-guide.md`](style-guide.md) para ver la paleta exacta y las especificaciones visuales.

## Aprendizajes

Este ejercicio permite practicar la maquetación de tarjetas, el uso de tipografías locales, la extracción de colores desde una referencia visual y la organización de CSS mediante LESS.