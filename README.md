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
y las monedas comienzan a almacenarse en la posición 1 de la matriz en lugar de cero, corregido restando 1 de todas las posiciones
Restringimos el método esJugable para que solo devuelva verdadero cuando el jugador tiene de 2 a 6.
El método add se modificó para depender del método esJugable.

## Problema 3

Se agregó una instrucción de jailbreak en el método tirarDado en caso de que arroje un número impar y vaya a la cárcel.
Creé la prueba "sacar_numero_impar_y_salir_de_la_cárcel" donde se burlará del inicio del juego
El jugador 1 va a la cárcel y sale después de una tirada extraña.
previsto.

## Problema 4

Dado que el método JugadorHaGanado es verdadero pero se completa sin un jugador todavía, cambiamos el nombre del método
Para JugadorNoHaGanado, cambiamos el nombre de la variable noGanador a Ganador.

## Problema 5

Refactorizamos el proceso de cambiar de jugador en el método pasarTurno y lo reemplazamos donde corresponde

