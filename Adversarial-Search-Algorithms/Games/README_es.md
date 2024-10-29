# Juegos 

En el campo de la inteligencia artificial y la teoría de juegos, los juegos son considerados una forma de interacción entre dos o más agentes (jugadores) que buscan maximizar sus ganancias o minimizar sus pérdidas en un entorno competitivo. Los juegos pueden clasificarse en varias categorías, siendo las más relevantes: 

1. **Juegos de suma cero**: En estos juegos, las ganancias de un jugador son exactamente iguales a las pérdidas de otro jugador. Un ejemplo clásico es el ajedrez.

2. **Juegos deterministas**: Estos juegos tienen un resultado predecible en función de las decisiones de los jugadores. No hay elementos de azar involucrados.

3. **Juegos simultáneos y secuenciales**: En los juegos simultáneos, los jugadores toman decisiones al mismo tiempo sin conocer las elecciones del otro. En los juegos secuenciales, los jugadores se turnan.

Los algoritmos de búsqueda en los juegos se centran en encontrar la mejor jugada posible explorando las posibles configuraciones del juego y evaluando el resultado de cada una.

--- 

## Implementación 

### 1. Tres en raya 
**Descripción**: Se trata de un juego para dos jugadores que se juega en un tablero de 3x3. Los jugadores colocan sus marcas (X u O) en un intento de alinear tres de sus marcas en una fila, columna o diagonal.

**Implementación simplificada**: 
- **Tablero**: Se crea un tablero vacío, representado como una lista de listas.
- **Turnos**: Los jugadores se turnan para introducir las coordenadas (fila y columna) donde quieren colocar su marca.
- **Verificación del ganador**: Después de cada movimiento, se comprueba si algún jugador ha conseguido alinear tres marcas (horizontal, vertical o diagonal). Si un jugador gana, el juego termina. Si el tablero está lleno sin un ganador, se declara un empate.

### 2. Nim 

**Descripción**: En este juego, hay varias pilas de palitos y los jugadores se turnan para quitar palitos de una pila. El objetivo es obligar al oponente a ser el que no pueda hacer un movimiento.

**Implementación simplificada**: 
- **Pilas**: Se inicializan varias pilas de palitos con diferentes cantidades.
- **Turnos**: Los jugadores eligen una pila y deciden cuántos palitos quitar (al menos uno, pero no más que la cantidad en la pila elegida).
- **Fin del juego**: El juego continúa hasta que no queden palitos en ninguna pila. El jugador que no pueda hacer un movimiento (porque todas las pilas están vacías) pierde.

--- 
## Conclusión 
Ambos juegos son ejemplos clásicos que ilustran conceptos importantes en la teoría de juegos y algoritmos de búsqueda. La implementación de estos juegos en Python permite una comprensión práctica de cómo funcionan los turnos, la verificación de la condición de victoria y la toma de decisiones estratégicas. Estos principios se pueden extender a juegos más complejos y a la creación de agentes que jueguen de manera efectiva.