# Style Guide — QR Code Component

Guía de los estilos **realmente utilizados** en la implementación HTML, CSS y LESS del componente QR.

## 1. Paleta de colores

Los colores se seleccionaron tomando muestras de la referencia visual con **PicPick**.

| Elemento | Color | Valor |
| --- | --- | --- |
| Fondo de la página | Azul grisáceo claro | `#D5E1EF` |
| Fondo de la tarjeta | Blanco | `#FFFFFF` |
| Texto del título | Azul oscuro | `#1B2A44` |
| Texto de la descripción | Gris oscuro | `#666666` |
| Sombra de la tarjeta | Gris claro | `#CCCCCC` |

Estos son los colores que aparecen en el CSS entregado; **no incluyen los azules y blancos internos del propio archivo de imagen QR**.

## 2. Tipografía

**Familia:** `Outfit`, con alternativa `sans-serif`.

**Origen:** archivo local `img/fonts/Outfit-VariableFont_wght.ttf`, declarado en CSS mediante `@font-face`.

| Elemento | Tamaño | Peso |
| --- | --- | --- |
| Título (`h1`) | `21px` | Negrita predeterminada del navegador (`h1`) |
| Descripción (`p`) | `14px` | Normal predeterminado del navegador (`p`) |

El CSS entregado **no define explícitamente** `font-weight` ni `line-height` para estos textos.

## 3. Tarjeta principal

| Propiedad | Valor |
| --- | --- |
| Ancho | `320px` |
| Fondo | `white` |
| Radio de esquinas | `20px` |
| Margen | `25vh auto` |
| Alineación de texto | `center` |
| Sombra | `0px 3px 5px #ccc` |

La tarjeta se centra **horizontalmente** mediante el margen automático. El margen vertical de `25vh` es el utilizado en el proyecto; no equivale a un centrado vertical exacto.

## 4. Imagen QR

| Propiedad | Valor |
| --- | --- |
| Ancho | `290px` |
| Alto | `auto` |
| Radio de esquinas | `10px` |
| Margen horizontal | `auto` |
| Margen superior | `20px` |

El selector utilizado en los archivos es `#qr-imgage`.

## 5. Título

- Selector: `#title`.
- Tamaño: `21px`.
- Color: `#1B2A44`.
- Ancho: `75%` del contenedor.
- `padding: 20px` y `padding-bottom: 15px`.
- Margen horizontal: `auto`.

## 6. Descripción

- Selector: `#description`.
- Tamaño: `14px`.
- Color: `#666666`.
- Ancho: `75%` del contenedor.
- `padding-bottom: 35px`.
- Margen horizontal: `auto`.

## 7. Variables LESS

```less
@bgcolor: #D5E1EF;
@font-family: 'Outfit', sans-serif;
@title-size: 21px;
@title-color: #1B2A44;
@description-size: 14px;
@description-color: #666;
```

El fondo blanco, el color de la sombra y los radios de las esquinas están escritos directamente en el archivo LESS, sin variables propias.

## 8. Comportamiento adaptable

El HTML incluye una etiqueta `viewport`, pero en el CSS entregado **no hay media queries**. El componente utiliza un ancho fijo de `320px`; por tanto, esta guía documenta la implementación actual y no atribuye comportamientos responsivos que no se hayan programado.
