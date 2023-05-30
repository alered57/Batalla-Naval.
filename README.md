# Batalla-Naval.
El programa que presentamos es un juego de batalla naval utilizando p5.js, una biblioteca de JavaScript para la creación de gráficos interactivos en el navegador.
//introducción + detalles clave de la implementación + resultados + conclusiones y trabajo futuro.

En este escrito se hara un breve resumen y una retroalimentacion del uso de javascript y su biblioteca p5 aplicado al diseño de juegos en 2D, mediante el uso de la logica de la biblioteca p5, hemos visto la utilidad y la facilidad con la que se puede lograr un diseño y modelado mediante archivos pregenerados, el uso de quadrillas y la implemtacion de archivos externos como fuentes en el programa.

Nuestro juego Batleship basicamente es un juego de estrategia para dos jugadores en el cual mediante una serie de roles se intenta destruir los barcos del otro jugador, en nuestro caso utilizamos a la maquina como rival basicamente se generan 5 barcos en posiciones aleatorias y mediante el uso del mouse se intentan encontrar dichos barcos, con un total de 50 clicks permitidos por partida, en un total de 100 cuadriculas permitidas para selecion, el juego cuenta con una pantalla principal donde se puede modular la musica y dar incio al juego como tal, basicamente una ambientacion, ya dentro la logica tras la programcion consta del uso de quadrillas sobrepuestas, por ejemplo los barcos, las posiciones y el tablero como tal, para la musica se usó un pista de internet recortada en formato mp3 la cual fue subida como fuente en el programa y luego implementada por la funcion loadSound, a partir de ahí se usó un bototn cuyo unico fin es el de interactuar con las propiedas play y stop, para la pantalla de inicio se usó un canvas adicional con un fondo de imagen como textura y dos botones, el de la musica mencionado con anterioridad, y el boton play el cual cumple la funcion de ejecutar el juego como tal, ya dentro del juego se generan 5 barcos al azar mediante el uso de la funcion random, y unas coordenadas limitadas al tamaño del tablero, cabe aclarar que cada barco es una cuadrilla diferente por ende se limitaron mediante los metodos de la cuadrilla para no generar sobreposicion, el tablero son tres cuadrilas como tal una vertical que indica las letras de la A - J, una horizontal que marca los numeros del 1 al 10, y por ultimo una cuadrilla de 11x11 donde se desarrolla el juego como tal (el tablero), detras del funcinamiento de los clicks se escuentra un funcion cuyo rol es el de detectar y redondear el valor del click y generar un cuadrado en dicha coordenada aproximada o un emoji si da en un barco, la puntuación funciona mediante un calculo entre el numero de clicks y la precicion al momento de apuntar, a aprtir de los 50 clicks salta la pantalla de game over, el cual es un canvas con una condicion ligada al puntaje, al igual que si logra destruir todos los barcos saltará una pantalla en verde donde dirá su puntaje y una felicitacion por su victoria tambien con un canvas con una condicion ligada al puntaje y al numero de clicks.

Como resultado tenemos un juego entretenido, que aplica la logica de las reglas de un juego retro en un ambiente mucho mas moderno, sin dejar de lado su escencia como juego de mesa


Como trabajo futuro sería la implemnetacion de una segunda pantalla para un juego multijugador en local, o en un entorno mas visionario desarrolar el juego con un multijugador online, ademas de agregar una serie de dificultades adicionales las cuales sean seleccionables, por ejemplo a mayor dificultad menor tamaño de los barcos entre otras cosas, en conclusion se logró dar una implemnetacion al conocimiento de manera satisfactoria dejando un programa que plasma nuestra creatividad y la aplicacion de los conocimientos a un entorno mas didactico como lo son los videojuegos















