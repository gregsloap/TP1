﻿# TP1-Bouncing Ball.
 
1.O projeto tem como objetivo aplicar os conhecimentos adquiridos sobre programação orientada a objetos, para simular o movimento de uma bola saltitante "bouncing ball".Tendo em vista que esseparadigma representa de maneira mais fiel objetos "fisicos" reais de modo a tratá-los de maneira mais intuitiva, sendo a bouncing-ball um exemplo ideal.
Para a realização do projeto foi necessária a utilização do Visual Studio 11(ou superior) em conjunto com o C++ lab, utilizando-se das bibliotecas: 

iostream
cmath
vector
cassert
algorithm
sstream
iomanip

A versão do compilador utilizada foi gcc 4.9.2.

Linhas de compilacao dos arquivos:

-test-ball : ball.cpp ball.h test-ball.cpp
-test-ball-graphics : graphics.cpp ball.cpp test-ball-graphics.cpp
-test-springmass : springmass.cpp test-springmass.cpp
-test-springmass-graphics : graphics.cpp springmass.cpp test-springmass-graphics.c 


Descrição dos arquivos:

- ball.h: Define a Classe ball e seus atributos que serão herdados por varias outras classes. 
- ball.cpp: Contem as coordenadas da bola e a implementaçao dos metodos para "movimentá-la" e mantém registro de sua posição.
- test-ball.cpp: Executa os metodos da ball.cpp, dando movimento de fato a bola.
- simulation.h: Define a Classe simulation e seus atributos; Contendo portanto as variáveis de ambiente necessárias para a representaçao física da "realidade" de modo a criar um ambiente para a simulação da bola quicando.
- spring-mass: define as variáveis e condiçoes necessarias para simular o "quique" emulando uma especie de força elástica que será aplicada ao "quique" da bola.
- test-spring-mass: executa os métodos, etc. Contidos na spring-mass.cpp
- test-spring.h: Define a Classe springmass:  e seus atributos que serão herdados por varias outras classes.

*obs:Os demais arquivos são referentes a interface e saída gráficas do program, essas já sendo pre-concebidas.



Task 2 (também no arquivo ball.txt) saída :
 0.01 -0.00877778
0.02 -0.0284444
0.03 -0.059
0.04 -0.100444
0.05 -0.152778
0.06 -0.216
0.07 -0.290111
0.08 -0.375111
0.09 -0.471
0.1 -0.577778
0.11 -0.695444
0.12 -0.824
0.13 -0.824
0.14 -0.695444
0.15 -0.577778
0.16 -0.471
0.17 -0.375111
0.18 -0.290111
0.19 -0.216
0.2 -0.152778
0.21 -0.100444
0.22 -0.059
0.23 -0.0284444
0.24 -0.00877778
0.25 -8.1532e-17
0.26 -0.00211111
0.27 -0.0151111
0.28 -0.039
0.29 -0.0737778
0.3 -0.119444
0.31 -0.176
0.32 -0.243444
0.33 -0.321778
0.34 -0.411
0.35 -0.511111
0.36 -0.622111
0.37 -0.744
0.38 -0.876778
0.39 -0.876778
0.4 -0.744
0.41 -0.622111
0.42 -0.511111
0.43 -0.411
0.44 -0.321778
0.45 -0.243444
0.46 -0.176
0.47 -0.119444
0.48 -0.0737778
0.49 -0.039
0.5 -0.0151111
0.51 -0.00211111
0.52 -4.90059e-16
0.53 -0.00877778
0.54 -0.0284444
0.55 -0.059
0.56 -0.100444
0.57 -0.152778
0.58 -0.216
0.59 -0.290111
0.6 -0.375111
0.61 -0.471
0.62 -0.577778
0.63 -0.695444
0.64 -0.824
0.65 -0.824
0.66 -0.695444
0.67 -0.577778
0.68 -0.471
0.69 -0.375111
0.7 -0.290111
0.71 -0.216
0.72 -0.152778
0.73 -0.100444
0.74 -0.059
0.75 -0.0284444
0.76 -0.00877778
0.77 -7.47666e-16
0.78 -0.00211111
0.79 -0.0151111
0.8 -0.039
0.81 -0.0737778
0.82 -0.119444
0.83 -0.176
0.84 -0.243444
0.85 -0.321778
0.86 -0.411
0.87 -0.511111
0.88 -0.622111
0.89 -0.744
0.89 -0.876778
0.88 -0.876778
0.87 -0.744
0.86 -0.622111
0.85 -0.511111
0.84 -0.411
0.83 -0.321778
0.82 -0.243444
0.81 -0.176
0.8 -0.119444
0.79 -0.0737778

Task 4:(no arquivo grafico.png)
