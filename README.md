# Investigación CSS

En este espació se encuentra la investigación de la tara de la semana:

## background-color:

Con esta propiedad se cambia el color de fondo del elemento html.

    html {
    background-color: blue;
    }

## color:

Con esta propiedad se le cambia el color al texto de un elemento.

    p {
        color: blueviolet;
    }

## border:

Con esta propiedad al elemento se le agrega un bode solido de un tamaño definido en pixeles color azul violeta.

    div {
        border: 2px solid yellowgreen;
    }

## Valores del Color:

En CSS, los colores también se pueden especificar usando valores RGB, valores HEX, valores HSL, valores RGBA y valores HSLA:

    div {
    background-color: rgb(red, green, blue);
    background-color: #fff;
    background-color: hsl(9, 100, 64);
    }

### RGB:

En CSS, un color se puede especificar como un valor RGB, utilizando esta fórmula: rgb (rojo, verde, azul),cada parámetro (rojo, verde y azul) define la intensidad del color entre 0 y 255.
Por ejemplo, rgb(255, 0, 0) se muestra como rojo, porque el rojo se establece en su valor más alto (255) y los demás se establecen en 0.

### Hexadecimal:

En CSS, se puede especificar un color usando un valor hexadecimal en la forma: #rrggbb, donde rr (rojo), gg (verde) y bb (azul) son valores hexadecimales entre 00 y ff (igual que decimal 0-255).
Por ejemplo, #ff0000 se muestra en rojo, porque el rojo se establece en su valor más alto (ff) y los demás se establecen en el valor más bajo (00).

### HSL

En CSS, un color se puede especificar utilizando el tono, la saturación y la luminosidad (HSL) en la forma: hsl(tono, saturación, luminosidad), El tono es un grado en la rueda de colores de 0 a 360. 0 es rojo, 120 es verde y 240 es azul. La saturación es un valor porcentual, 0 % significa un tono de gris y 100 % es el color completo. La luminosidad también es un porcentaje, el 0 % es negro, el 50 % no es ni claro ni oscuro, el 100 % es blanco.

## Fondos CSS:

### background-color:

Está propiedad especifica el color de fondo de un elemento.

    body {
    background-color: lightblue;
    }

#### opacity

La propiedad especifica la opacidad/transparencia de un elemento. Puede tomar un valor de 0.0 - 1.0. Cuanto menor sea el valor, más transparente.

    div {
    background-color: green;
    opacity: 0.3;
    }

    div {
    background: rgba(0, 128, 0, 0.3) /* Green background with 30% opacity */
    }

### background-image:

Está propiedad especifica una imagen para usar como fondo de un elemento, tiene que referenciar bien la ruta en donde se encuentra la imagen.

    body {
    background-image: url("paper.gif");
    }

### background-repeat:

Está propiedad repite una imagen tanto horizontal como verticalmente, Algunas imágenes deben repetirse solo horizontal o verticalmente, o se verán extrañas.

    body {
    background-image: url("gradient_bg.png");
    }

Para que solo se repita horizontalmente:

    body {
    background-image: url("gradient_bg.png");
    background-repeat: repeat-x;
    }

Para que solo se repita verticalmente:

    body {
    background-image: url("gradient_bg.png");
    background-repeat: repeat-y;
    }

La propiedad también especifica mostrar la imagen de fondo solo una vez:

    body {
    background-image: url("img_tree.png");
    background-repeat: no-repeat;
    }

#### Posición de Fondos CSS

Está propiedad se utiliza para especificar la posición de la imagen de fondo, en el ejemplo
se coloca la imagen en la esquina superior derecha.

    body {
    background-image: url("img_tree.png");
    background-repeat: no-repeat;
    background-position: right top;
    }

### background-attachment:

Está propiedad especifica si la imagen de fondo debe desplazarse o ser fija (no se desplazará con el resto de la página), en el ejemplo la imagen es fija.

    body {
    background-image: url("img_tree.png");
    background-repeat: no-repeat;
    background-position: right top;
    background-attachment: fixed;
    }

En el ejemplo la imagen de fondo debe desplazarse con el resto de la página.

    body {
    background-image: url("img_tree.png");
    background-repeat: no-repeat;
    background-position: right top;
    background-attachment: scroll;
    }

### background:

Para acortar el código, también es posible especificar todas las propiedades de fondo en una sola propiedad. Esto se llama una propiedad abreviada.

Forma normal:

    body {
    background-color: #ffffff;
    background-image: url("img_tree.png");
    background-repeat: no-repeat;
    background-position: right top;
    }

Forma abreviada:

    body {
    background: #ffffff url("img_tree.png") no-repeat right top;
    }
