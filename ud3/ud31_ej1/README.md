### 1. Position: static
El cuadro 1 no se mueve al añadir left: 50px.
Esto ocurre porque static es el valor predeterminado de position y no permite utilizar las propiedades top, right, bottom y left para desplazar el elemento.

### 2. Position: relative
El cuadro 2 se desplaza 20 píxeles hacia abajo y 50 píxeles hacia la derecha.
Aunque se mueve visualmente, conserva su espacio original en la página. Por eso deja un hueco en su posición inicial.

### 3. Position: absolute
Al utilizar position: absolute, el cuadro 3 sale del flujo normal de la página y deja de reservar su espacio original.
Sin position: relative en el contenedor, el cuadro se posiciona respecto al bloque contenedor de referencia de la página.
Al añadir position: relative al contenedor, el cuadro se coloca en su esquina superior derecha.
Los demás cuadros no ocupan un hueco para el cuadro 3 porque este ya no forma parte del flujo normal.

### 4. Z-index
He utilizado top: -40px para desplazar el cuadro 2 hacia arriba y conseguir que se solape con el cuadro 1.
Después he utilizado z-index para controlar el orden de los cuadros.
El cuadro 1 tiene z-index: 2 y el cuadro 2 tiene z-index: 1. Por eso el cuadro 1 aparece por encima del cuadro 2.

## Conclusión
He aprendido que position permite controlar la posición de los elementos de una página.
- static: posición normal.
- relative: permite desplazar el elemento sin perder su espacio original.
- absolute: saca el elemento del flujo normal y lo posiciona respecto a su bloque contenedor de referencia.
- z-index: controla el orden de superposición de los elementos posicionados.
