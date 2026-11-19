#Flex

Dos ejes: principal y cruzado
Eje principal: la dirección en la que se
colocan los ítems.
Eje cruzado: el perpendicular al principal.
flex-direction elige el principal.
Por defecto es row (horizontal).
flex-direction: row
flex-direction: column
flex-direction: row-reverse
flex-direction: column-reverse

flex-start
center
flex-end
space-between
space-around
space-evenly

gap y flex-wrap: separar y saltar de línea
.tarjetas {
display: flex;
flex-wrap: wrap;
gap: 16px;
}
Sin flex-wrap, los ítems se encogen para caber en una sola línea. gap sustituye a los margin entre elementos y no deja hueco en los extremos.

.portada {
display: flex;
justify-content: center;
align-items: center;
height: 300px;
}

.platos {
display: flex;
gap: 16px;
}
.platos article {
flex: 1;
}
