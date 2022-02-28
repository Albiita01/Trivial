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

## Problema 4
En la clase "Game Launcher", cambiamos donde pone "noGanador" por "ganador" y lo convertimos 
en variable para que ahora ganador sea true y se acabe la partida.

## Problema 5
En la clase Game, busco cuál es el código para pasar al siguiente jugador y veo que es: 
"jugadorActual++;
if (jugadorActual == jugadores.size()) jugadorActual = 0;"
Lo selecciono y le doy a "Refactor" y luego a "Extract method", le pongo el nombre de "siguienteJuugador()" 
al método y lo sustituyo en todos los sitios que aparezca.

## Problema 6
En el método "fueRespuestaCorrecta()", busco lo que está repetido, que es:
"System.out.println("Respuesta correcta!!!!");
monederos[jugadorActual]++;
System.out.println(jugadores.get(jugadorActual)
+ " ahora tiene "
+ monederos[jugadorActual]
+ " monedas doradas.");

boolean ganador = jugadorHaGanado();
siguienteJugador();

return ganador;"
Lo selecciono todo y le doy a "Refactor" y luego a "Extract method", le pongo el nombre de "respCorrecta()" 
y lo sustituyo en ambos lados.