# Trivial

## Problema 0
Extraemos el código duplicado a un único método "nuevaPosicionJugador", 
al que llamamos desde ambos sitios.

Creamos test unitario "si_al_principio_saco_un_1_voy_a_casilla_1()"

## Problema 1
En el método "esJugable()" creamos las condiciones de si el número de jugadores es 
menor que 2, devuelve false, y en caso contrario, devuelve true. He hecho dos tests 
uno que prueba cuando los jugadores son menos de 2 ("menosDeDosJugadores()") 
y otro que prueba que los jugadores son 2 ("dosJugadores()").