# Trivial

## Problema 0

Extraemos el código duplicado a un único método "nuevaPosicionJugador",
al que llamamos desde ambos sitios.
Creamos test unitario "si_al_principio_saco_un_1_voy_a_casilla_1"

## Problema 1
El método esJugable se utiliza como condición para iniciar el juego.
Si esto no es posible, aparecerá un mensaje indicando que el número de jugadores es incorrecto.
Además, creamos la prueba unitaria "si_hay_menos_de_2_jugadores" para la verificación.
## Problema 2

Creamos una prueba para probar 6 jugadores y encontramos que hay un error porque la posición
y las monedas comienzan a almacenarse en la posición 1 de la matriz en lugar de cero, corregido
restando 1 de todas las posiciones. Restringimos el método esJugable para que solo devuelva
verdadero cuando el jugador tiene de 2 a 6. El método add se modificó para depender del método esJugable.

## Problema 3

Añado la instrucción de salir de la cárcel en el método tirarDado en el supuesto de sacar un
número impar y estar en la cárcel. Creo el test  sacar_numero_impar_y_salir_de_la_cárcel 
donde simulo un principio de partida donde el jugador 1 va a la cárcel y sale después de
sacar un número impar avanzando hasta la casilla esperada.

## Problema 4

Dado que el método JugadorHaGanado es verdadero pero se completa sin un jugador todavía,
cambiamos el nombre del método. Para JugadorNoHaGanado, cambiamos el nombre de la variable
noGanador a Ganador.

## Problema 5

Refactorizamos el proceso de cambiar de jugador en el método pasarTurno y lo
reemplazamos donde corresponde

# Problema 6

Extraemos la parte correcta de la pregunta del método fueRespuestaCorrecta y 
llamamos al nuevo método respuestaAcertada. Reutilizarlo en la segunda parte 
del método fueRespuestaCorrecta.

## Problema 7

Agregamos el comando addLast en el método hacerPregunta para agregar las preguntas
descartadas al final de la lista Este tipo de pregunta utiliza una variable que 
descarta el contenido de la pregunta y el código es
ver más claro.

Luego creamos una nueva prueba llamada hacer_mas_de_50_preguntas donde usamos un bucle for
para preguntar más de 50 preguntas, puede ver en la pantalla que la lista comienza de 
nuevo con la pregunta 0.