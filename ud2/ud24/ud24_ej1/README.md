## Display utilizado
He elegido display: flex en el contenedor `.contenido` porque permite colocar las tres tarjetas en una misma fila de forma sencilla y organizada.

### 1. ¿Qué diferencia hay entre margin y padding?
Padding es el espacio interior entre el contenido y el borde de una caja.
Margin es el espacio exterior que separa una caja de los demás elementos.

### 2. ¿Por qué saltaba la tercera tarjeta de línea?
Porque las tres tarjetas ocupaban más espacio del disponible.
Cada tarjeta tenía 220px de ancho, 30px de padding, 2px de borde y 20px de margin. En total eran 272px por tarjeta.
Las tres tarjetas necesitaban 816px, por lo que no cabían en el espacio disponible.
Lo solucioné reduciendo el ancho a 200px y el margin a 5px.

### 3. ¿Qué propiedades ignoraba el span y por qué?
El span es un elemento en línea por defecto.
Por eso no se aplicaban width ni height, y los márgenes verticales tampoco modificaban la separación de las líneas.
Al utilizar display: inline-block, pude controlar su anchura, altura y márgenes.

### 4. ¿Qué hace display: none con el espacio que ocupaba la caja?
Hace que el elemento desaparezca completamente de la página y que no reserve espacio.
Las demás tarjetas ocupan el espacio disponible.
