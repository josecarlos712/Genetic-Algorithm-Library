## Inteligencia Artificial

### Práctica 2

- Álvaro Aguayo Orozco
- Javier Blasco Vázquez
- Jose Carlos Crespo Falcon

### Introducción

El objetivo de esta segunda práctica es extender las funcionalidades de la librería de algoritmos genéticos, con nuevos métodos de selección, cruzamiento y mutación.

### Métodos de Selección

##### Elitista

Se trata de un mecanismo mediante el cual los mejores elementos de una población se mantienen intactos en la siguiente.

##### Rulette

Los padres se escogen en base a su fitness, los elementos con mejor fitness tienen más posibilidades de ser escogidos.

##### Rango

Similar a la ruleta, pero ahora los elementos se ordenan según su ranking. Si contamos con n elementos, el peor tendrá un valor de 1 y el que tenga el mejor la n. 

##### Natural

Funcionamiento estándar de la librería.

### Métodos de Cruzamiento

##### Single-Point

De los dos cromosomas, se escoge un punto al azar entre el tamaño de los mismos. Después, se intercambia la información de dicho punto hacia adelante y hacia atrás para formar hijos que combinen la información de los dos padres.

##### Two-Point

Similar al caso anterior, pero ahora el corte se realiza por dos puntos diferentes y tomados también al azar.

##### Uniform

En el cruzamiento uniforme cada gen del cromosoma puede ser escogido de cualquiera de los dos padres al azar (con igualdad de posibilidades).

##### Uniform-media

Es una variante del uniform en el que nos aseguramos que la cantidad de genes que se intercambian sean exactamente la mitad de los genes distintos.

##### Ordered

Es un método específico para cuando el problema trata de genomas de listas ordenadas. Para el funcionamiento se crean sublistas de los cromosomas, comprobando los elementos de este que faltan en el otro y añadiéndolos en el orden en el que nos lo encontramos.

### Métodos de Mutación

##### Flip

Es el método por defecto de la librería. Muta o no un gen del cromosoma arbitrariamente dependiendo del porcentaje de mutación.

##### Scramble

Escoge, en base al ratio de mutación, una sublista de genes y los desordena de manera aleatoria.

##### Inversión

Parecido al anterior, solo que en lugar de desordenarla de manera aleatoria lo que hace es invertir una sublista de genes.

##### Gamma

Muta un gen aleatorio del cromosoma y le asigna un valor según una distribución gamma.
