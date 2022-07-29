# Investigación CSS

En este espació se encuentra la investigación de la tara de la semana:

## color:

Con esta propiedad se le cambia el color al texto de un elemento.

    p {
        color: blueviolet;
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

## background-color:

Está propiedad especifica el color de fondo de un elemento.

    body {
    background-color: lightblue;
    }

### Opacity

La propiedad especifica la opacidad/transparencia de un elemento. Puede tomar un valor de 0.0 - 1.0. Cuanto menor sea el valor, más transparente.

    div {
    background-color: green;
    opacity: 0.3;
    }

    div {
    background: rgba(0, 128, 0, 0.3) /* Green background with 30% opacity */
    }

## background-image:

Está propiedad especifica una imagen para usar como fondo de un elemento, tiene que referenciar bien la ruta en donde se encuentra la imagen.

    body {
    background-image: url("paper.gif");
    }

## background-repeat:

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

### Posición de Fondos CSS

Está propiedad se utiliza para especificar la posición de la imagen de fondo, en el ejemplo
se coloca la imagen en la esquina superior derecha.

    body {
    background-image: url("img_tree.png");
    background-repeat: no-repeat;
    background-position: right top;
    }

## background-attachment:

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

## background:

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

## Borde CSS

Las propiedades de borde de CSS permiten especificar el estilo, el ancho y el color del borde de un elemento.

## border-style:

Está propiedad especifica qué tipo de borde mostrar, puede tener de uno a cuatro valores (para el borde superior, el borde derecho, el borde inferior y el borde izquierdo).

- dotted: Define un borde punteado
- dashed: Define un borde discontinuo
- solid: Define un borde sólido
- double: Define un borde doble
- groove: Define un borde ranurado 3D. El efecto depende del valor del color del borde.
- ridge: Define un borde estriado 3D. El efecto depende del valor del color del borde.
- inset: Define un borde de inserción 3D. El efecto depende del valor del color del borde.
- outset: Define un borde inicial 3D. El efecto depende del valor del color del borde.
- none: No define ningún borde
- hidden: Define un borde oculto

```
  p {
  border-style: dotted;
  }

  p {
  border-style: dashed;
  }

  p {
  border-style: solid;
  }

  p {
  border-style: double;
  }

  p {
  border-style: groove;
  }

  p {
  border-style: ridge;
  }

  p {
  border-style: inset;
  }

  p {
  border-style: outset;
  }

  p {
  border-style: none;
  }

  p {
  border-style: hidden;
  }

  p {
  border-style: dotted dashed solid double;
  }
```

## border-width:

Está propiedad puede tener de uno a cuatro valores (para el borde superior, el borde derecho, el borde inferior y el borde izquierdo):

css```
p.one {
border-style: solid;
border-width: 5px 20px; /_ 5px top and bottom, 20px on the sides _/
}

    p.two {
    border-style: solid;
    border-width: 20px 5px; /* 20px top and bottom, 5px on the sides */
    }

    p.three {
    border-style: solid;
    border-width: 25px 10px 4px 35px; /* 25px top, 10px right, 4px bottom and 35px left */
    }

```

```
