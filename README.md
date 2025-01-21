# 🎮 Connect 4 game: reinforcement learning

## Objetivo: Desarrollar un agente de aprendizaje por refuerzo para el juego de connect4.

Connect4 consiste en un juego entre dos jugadores (i.e., agentes), rojo y amarillo, con el objetivo de hacer una línea recta de 4 fichas del mismo color. La líneas pueden ser verticales, horizontales o diagonales. El tablero del juego se define como una cuadrícula de 6 filas y 7 columnas. Cada casilla del tablero puede tener una ficha roja, una ficha amarilla o estar vacía. Por último, cada jugador tiene 21 fichas para jugar en el tablero.

La dinámica del juego se desarrollo por turnos, cualquiera de los jugadores puede comenzar y jugarán una ficha a la vez intercaladamente hasta que exista un ganador o hasta que no queden más fichas por jugar.

En cada jugada, el jugador de turno, pone una ficha en la primera casilla disponible (de abajo a arriba) en una columna específica.

El agente de aprendizaje por refuerzo pueda jugar connect4 con un humano u otro agente. Más aún, el agente debe poder desempeñarse como primer jugador o como segundo jugador.

## Descripción del entorno

### Agente 

En el juego participan dos jugadores, uno representa las fichas de color rojo y el otro las de color amarillo. El agente de aprendizaje por refuerzo es un algoritmo que intenta aprender la mejor estrategia para ganar el juego, este puede jugar Connect 4 contra un humano o contra otro agente.

### Entorno

El entorno incluye el tablero de juego, las fichas de los jugadores y las reglas del juego.

- El tablero: está representado por una cuadrícula de 6 filas y 7 columnas, donde se colocan las fichas.

- Las fichas del juego: cada jugador dispone de 21 fichas de un color (rojas o amarillas).

- Las reglas de juego:

• El objetivo de Connect 4 es alinear cuatro fichas sobre el tablero.

• Cualquiera de los jugadores puede comenzar.

•  Por turnos, cada jugador debe colocar una ficha en la columna de su elección, siempre que ésta no esté llena. La ficha caerá hasta la posición más baja disponible, siguiendo la ley de la gravedad. Es importante destacar que no se puede perder el turno; cada jugador debe realizar su movimiento en el momento correspondiente. Asimismo, una vez que la ficha ha sido colocada, no podrá ser retirada del tablero.

• Gana la partida el primero que consiga alinear cuatro fichas consecutivas de un mismo color en horizontal, vertical o diagonal.

• Si todas las columnas están llenas, pero nadie ha hecho una alineación válida, hay empate.





