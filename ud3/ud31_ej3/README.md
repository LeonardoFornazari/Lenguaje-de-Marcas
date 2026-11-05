## Parte A - Etiqueta sobre la tarjeta
Position: relative en la tarjeta para que la etiqueta se coloque respecto a ella.
La etiqueta utiliza position: absolute, top: -10px y right: -10px para situarse en la esquina superior derecha y sobresalir un poco.

### ¿Qué ocurre al añadir overflow: hidden?
La parte de la etiqueta que sobresale de la tarjeta queda recortada.
Esto ocurre porque overflow: hidden oculta el contenido que sale de los límites de la caja.
Para solucionarlo, he quitado overflow: hidden de la tarjeta. Así la etiqueta puede sobresalir sin quedar recortada.

## Parte B - Caja de comentarios
- visible: muestra el contenido que sobresale de la caja.
- hidden: oculta el contenido que no cabe.
- scroll: permite desplazarse por el contenido mediante barras de desplazamiento.
- auto: muestra las barras de desplazamiento cuando son necesarias.
Finalmente, he dejado overflow: auto.

## Diferencia entre visibility: hidden y display: none
- visibility: hidden: oculta la tarjeta visualmente, pero conserva el espacio que ocupaba.
- display: none: elimina la tarjeta de la página y no reserva espacio.
Por eso, con display: none, las demás tarjetas pueden ocupar el espacio que queda libre.
