# Batalla-Naval.
El programa que presentamos es un juego de batalla naval utilizando p5.js, una biblioteca de JavaScript para la creación de gráficos interactivos en el navegador.

Introducción:

A continuación se dará un resumen y una retroalimentación del uso de javascript y su biblioteca p5 aplicado al diseño de juegos en 2D. Usando la lógica de la biblioteca p5, hemos visto la utilidad y la facilidad con la que se puede lograr un diseño y modelado mediante archivos pregenerados, el uso de quadrillas y la implementación de archivos externos como fuentes en el programa.

Implementación:

Es un juego de estrategia para dos jugadores en el cual a través de una serie de roles se intenta destruir los barcos del otro jugador, y en nuestro caso, utilizamos a la máquina como rival. Se generan 5 barcos en posiciones aleatorias y por medio del uso del mouse se intentan encontrar dichos barcos, con un total de 50 clicks permitidos por partida, en un total de 100 cuadriculas permitidas para selección. 

El juego cuenta con una pantalla principal donde se puede modular la música y dar inicio al juego. La lógica detrás de la programacion consta del uso de quadrillas sobrepuestas, por ejemplo los barcos, las posiciones y el tablero. Para la musica se usó una pista de internet recortada en formato mp3, la cual fue subida como fuente en el programa y luego implementada por la funcion loadSound. A partir de ahí, se usó un botón cuyo único fin es el de interactuar con las propiedades play y stop. 

Para la pantalla de inicio se usó un canvas adicional con un fondo de imagen como textura y dos botones, el de la música mencionado con anterioridad, y el boton play para ejecutar el juego. Ya dentro del juego se generan 5 barcos al azar mediante el uso de la funcion random y unas coordenadas limitadas al tamaño del tablero; cabe aclarar que cada barco es una cuadrilla diferente, por ende se limitaron empleando los métodos de la cuadrilla para no generar sobreposición. El tablero son tres cuadrillas, de las cuales una es vertical que indica las letras de la A - J, una horizontal que marca los números del 1 al 10, y por último una cuadrilla de 11x11 donde se desarrolla el juego (el tablero). 

Detrás del funcinamiento de los clicks se encuentra una función cuyo rol es el de detectar y redondear el valor del click, así mismo generar un cuadrado en dicha coordenada aproximada o un emoji si da en un barco. La puntuación funciona mediante un cálculo entre el número de clicks y la precisión al momento de apuntar, a partir de los 50 clicks salta la pantalla de game over, el cual es un canvas con una condición ligada al puntaje. Al igual que si logra destruir todos los barcos saltará una pantalla en verde donde dirá su puntaje y una felicitación por su victoria, también con un canvas con una condición ligada al puntaje y al número de clicks.

Resultados:

Tenemos un juego entretenido, que aplica la lógica de las reglas de un juego retro en un ambiente mucho mas moderno, sin dejar de lado su esencia como juego de mesa.

Trabajo futuro:

Como trabajo futuro sería la implementación de una segunda pantalla para un juego multijugador en local, o en un entorno más visionario desarrollar el juego con un multijugador online, ademas de agregar una serie de dificultades adicionales las cuales sean seleccionables. Por ejemplo, a mayor dificultad menor tamaño de los barcos entre otras cosas. En conclusion, se logró dar una implementación al conocimiento de manera satisfactoria dejando un programa que plasma nuestra creatividad y la aplicación de los conocimientos adquiridos para ofrecer una experiencia de juego entretenida y desafiante.















