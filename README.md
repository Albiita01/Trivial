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

## Problema 2
En el método "esJugable()" creamos la condición de si los jugadores son más de 6, 
que devuelva false. En los tests, he creado varios tests. El primero comprueba 
que los jugadores sean entre 2 y 6; el segundo comprueba que haya 6 jugadores y el 
último, que haya más de 6 jugadores.

## Problema 3
En el método "tirarDado()", ponemos las llaves correspondientes después del tercer 
if para que el jugador pueda salir de la cárcel y continuar con la partida. En 
la clase de los tests, he creado un test "salirDeLaCarcel()" que simula una partida para comprobar 
que ya se puede salir de la cárcel si el jugador acierta la pregunta.