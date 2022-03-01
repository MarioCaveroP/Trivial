# Trivial

## Problema 0

Extraemos el código duplicado a un único método "nuevaPosicionJugador",
al que llamamos desde ambos sitios.

Creamos test unitario "si_al_principio_saco_un_1_voy_a_casilla_1"

## Problema 1
Se usa el método esJugable como condición para que el juego sea lanzado.
De no ser posible, aparecerá un mensaje indicando que el número de jugadores es incorrecto.
Ademas, creamos el test unitario "si_hay_menos_de_2_jugadores" para su comprobación.

## Problema 2

Creamos el test para probar con 6 jugadores y nos encontramos que hay un error porque las posiciones
y las monedas se empiezan a guardar en la posición del array 1 y no en la cero, se corrige restando 1 a todas las posiciones
y limitamos el método esJugable para que solo devuelva true si los jugadores son de 2 a 6.
El método agregar se modifica para que dependa del método esJugable.

## Problema 3

Se añade la instruccion salir de la carcel en el metodo tirarDado por si saca un numero impar y esta en la carcel
Creo el test  sacar_numero_impar_y_salir_de_la_cárcel donde se simulara el principio de partida donde
el jugador 1 va a la cárcel y sale después de sacar un número impar avanzando hasta la casilla
esperada.