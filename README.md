 # Trabalho 1 Técnicas de programação 1.
 ## Universidade de Brasília
 ### Departamento de Ciencias da Computação
 #### Professor: Téofilo de Campos
 
 
 #### Aluno: João Gregório Mesquita Saiz Lopes
 #### Matrícula:15/0132018
 #### Turma: A.
### 1.0 Ball 
### 1.1. Introdução: 
O projeto tem como objetivo aplicar os conhecimentos adquiridos sobre programação orientada a objetos, para simular o movimento de uma bola saltitante "bouncing ball".Tendo em vista que esseparadigma representa de maneira mais fiel objetos "fisicos" reais de modo a tratá-los de maneira mais intuitiva, sendo a bouncing-ball um exemplo ideal.
### 1.2. Requisitos:
- Para a realização do projeto foi necessária a utilização do Visual Studio 11(ou superior) em conjunto com o C++ lab, utilizando-se das bibliotecas: 

		iostream
		cmath
		vector
		cassert
		algorithm
		sstream
		iomanip

- A versão do compilador utilizada foi gcc 4.9.2.

- Linhas de compilacao dos arquivos:

	 	cd < diretório > 

		g++ ball.cpp ball.h test-ball.cpp -o ball 

### 1.3. Descrição dos arquivos:

- **ball.h:** Define a Classe ball seus métodos e atributos que serão utilizados na criação dos objetos .

	**Atributos de ball:** Posição e velocidade no eixo x e y, raio e massa, gravidade aplicada e as dimensões da caixa onde a bola 	se encontra; 

	**Métodos de ball:** 

		Step: Calcula o passo da bola. 
		
		Display: Imprime os valores na tela.
		
- **ball.cpp:** Contem as coordenadas da bola e a implementaçao dos metodos para "movimentá-la" e mantém registro de sua posição.
- **test-ball.cpp:** Executa os metodos da ball.cpp, dando movimento de fato a bola.
- **springmass.h:**
- **springmass.cpp** 
- **simulation-test.cpp**


### 1.4. Diagrama: 

![diagrama de classes](https://github.com/gregsloap/TP1/blob/master/diagramadeclasses.png)


### 1.5. Saída de *ball.h*
- obs: Task 2 (também no arquivo [ball.txt](https://github.com/gregsloap/TP1/blob/master/ball.txt)):


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

### 1.6. Gráfico:

	obs: Task 4

![grafico.png](https://github.com/gregsloap/TP1/blob/master/grafico.png)

- gráfico produzido com plotly, segue o link: https://plot.ly/~gregfla2009/3/
### 2.0 Spring 
### 2.1 Introdução:
Continuando o que foi feito em *Ball*, essa parte do trabalho visa implementar uma forma de descrever a mola, seu percurso e comportamento, agora possuindo uma massa em cada ponta, retornando as respectivas coordenadas referentes ao comportamento da mola em questão.
### 2.2 Pré-Requisitos:
- Para a realização dessa etapa do trabalho foram necessarias as bibliotecas a seguir:
		
		iostream 
		springmass (contém a classe massa e classe mola, também usado na etapa anterior)
		simulation (contém a classe abstrata simulation)
		
- A versão do compilador utilizada foi gcc 4.9.2.
- Linhas de compilacao dos arquivos:

		cd < diretório > 

		g++ springmass.cpp test-springmass.cpp
		
### 2.3. Descrição dos arquivos:

- **springmass.h:** Define a Classe springmass seus métodos e atributos a serem utilizados na criação dos objetos .

	**Atributos de spring:** Coeficiente de amortecimento da mola, bem como seu Comprimento(deformação), Rigidez(resistencia a deformacao), as Massas a serem adicionadas em suas ponta, bem como a energia aplicada sobre si e sua força; 

	**Métodos de spring:** 

		Step: Calcula o passo da mola. 
		
		Display: Imprime os valores de saída.
		
- **springmass.cpp:** Contem as coordenadas da mola e a implementaçao dos metodos para "movimentá-la" e mantém registro de sua posição.
- **test-springmass.cpp:** Cria-se o Objeto e são executados os metodos da classe springmass, dando movimento de fato a mola.

### 2.4. Diagrama: 

![diagrama de classes](https://github.com/gregsloap/TP1/blob/master/diagramadeclasses2.png)

### 2.5. Saída de ***spring*** :
			
	energia total: 0.175914
	X1: -0.5 Y1: 0.104953
	X2: 0.5 Y2: 0.0991
	energia total: 0.310829
	X1: -0.499951 Y1: 0.938807
	X2: 0.500146 Y2: 0.928932
	energia total: 0.311291
	X1: -0.499902 Y1: 0.938807
	X2: 0.500391 Y2: 0.928932
	energia total: 0.310704
	X1: -0.499815 Y1: 0.938807
	X2: 0.500847 Y2: 0.928932
	energia total: 0.311328
	X1: -0.499728 Y1: 0.938807
	X2: 0.501479 Y2: 0.928932
	energia total: 0.310754
	X1: -0.499639 Y1: 0.938807
	X2: 0.502288 Y2: 0.928932
	energia total: 0.311395
	X1: -0.49955 Y1: 0.938807
	X2: 0.503279 Y2: 0.928932
	energia total: 0.310837
	X1: -0.499458 Y1: 0.938807
	X2: 0.504453 Y2: 0.928932
	energia total: 0.311497
	X1: -0.499365 Y1: 0.938807
	X2: 0.505816 Y2: 0.928932
	energia total: 0.310955
	X1: -0.49927 Y1: 0.938807
	X2: 0.507372 Y2: 0.928932
	energia total: 0.311639
	X1: -0.499172 Y1: 0.938807
	X2: 0.509126 Y2: 0.928932
	energia total: 0.311118
	X1: -0.499071 Y1: 0.938807
	X2: 0.511085 Y2: 0.928932
	energia total: 0.311828
	X1: -0.498967 Y1: 0.938807
	X2: 0.513255 Y2: 0.928932
	energia total: 0.311332
	X1: -0.498859 Y1: 0.938807
	X2: 0.515644 Y2: 0.928932
	energia total: 0.312076
	X1: -0.498748 Y1: 0.938807
	X2: 0.51826 Y2: 0.928932
	energia total: 0.311611
	X1: -0.498632 Y1: 0.938807
	X2: 0.521113 Y2: 0.928932
	energia total: 0.312395
	X1: -0.498511 Y1: 0.938807
	X2: 0.524212 Y2: 0.928932
	energia total: 0.31197
	X1: -0.498385 Y1: 0.938807
	X2: 0.527568 Y2: 0.928932
	energia total: 0.312804
	X1: -0.498253 Y1: 0.938807
	X2: 0.531193 Y2: 0.928932
	energia total: 0.31243
	X1: -0.498115 Y1: 0.938807
	X2: 0.5351 Y2: 0.928932
	energia total: 0.313325
	X1: -0.497971 Y1: 0.938807
	X2: 0.539303 Y2: 0.928932
	energia total: 0.313015
	X1: -0.497819 Y1: 0.938807
	X2: 0.543816 Y2: 0.928932
	energia total: 0.313988
	X1: -0.49766 Y1: 0.938807
	X2: 0.548656 Y2: 0.928932
	energia total: 0.313759
	X1: -0.497492 Y1: 0.938807
	X2: 0.553839 Y2: 0.928932
	energia total: 0.31483
	X1: -0.497316 Y1: 0.938807
	X2: 0.559384 Y2: 0.928932
	energia total: 0.314704
	X1: -0.49713 Y1: 0.938807
	X2: 0.565311 Y2: 0.928932
	energia total: 0.315899
	X1: -0.496933 Y1: 0.938807
	X2: 0.571642 Y2: 0.928932
	energia total: 0.315904
	X1: -0.496726 Y1: 0.938807
	X2: 0.578398 Y2: 0.928932
	energia total: 0.317256
	X1: -0.496506 Y1: 0.938807
	X2: 0.585605 Y2: 0.928932
	energia total: 0.317429
	X1: -0.496274 Y1: 0.938807
	X2: 0.593289 Y2: 0.928932
	energia total: 0.318979
	X1: -0.496028 Y1: 0.938807
	X2: 0.601478 Y2: 0.928932
	energia total: 0.319366
	X1: -0.495768 Y1: 0.938807
	X2: 0.610202 Y2: 0.928932
	energia total: 0.32117
	X1: -0.495492 Y1: 0.938807
	X2: 0.619496 Y2: 0.928932
	energia total: 0.32183
	X1: -0.495199 Y1: 0.938807
	X2: 0.62939 Y2: 0.928932
	energia total: 0.323957
	X1: -0.494887 Y1: 0.938807
	X2: 0.639927 Y2: 0.928932
	energia total: 0.324969
	X1: -0.494557 Y1: 0.938807
	X2: 0.651144 Y2: 0.928932
	energia total: 0.327509
	X1: -0.494205 Y1: 0.938807
	X2: 0.663086 Y2: 0.928932
	energia total: 0.328972
	X1: -0.493831 Y1: 0.938807
	X2: 0.675799 Y2: 0.928932
	energia total: 0.332044
	X1: -0.493431 Y1: 0.938807
	X2: 0.689337 Y2: 0.928932
	energia total: 0.334089
	X1: -0.493006 Y1: 0.938807
	X2: 0.703752 Y2: 0.928932
	energia total: 0.337848
	X1: -0.49255 Y1: 0.938807
	X2: 0.719106 Y2: 0.928932
	energia total: 0.34065
	X1: -0.492065 Y1: 0.938807
	X2: 0.735462 Y2: 0.928932
	energia total: 0.345302
	X1: -0.491544 Y1: 0.938807
	X2: 0.752896 Y2: 0.928932
	energia total: 0.349093
	X1: -0.490987 Y1: 0.938807
	X2: 0.77148 Y2: 0.928932
	energia total: 0.354913
	X1: -0.490387 Y1: 0.938807
	X2: 0.791305 Y2: 0.928932
	energia total: 0.360005
	X1: -0.489744 Y1: 0.938807
	X2: 0.812461 Y2: 0.928932
	energia total: 0.367371
	X1: -0.489049 Y1: 0.938807
	X2: 0.835057 Y2: 0.928932
	energia total: 0.374196
	X1: -0.488301 Y1: 0.938807
	X2: 0.859202 Y2: 0.928932
	energia total: 0.383629
	X1: -0.48749 Y1: 0.938807
	X2: 0.885034 Y2: 0.928932
	energia total: 0.39279
	X1: -0.486611 Y1: 0.938807
	X2: 0.912689 Y2: 0.928932
	energia total: 0.40503
	X1: -0.485654 Y1: 0.938807
	X2: 0.942339 Y2: 0.928932
	energia total: 0.417397
	X1: -0.484611 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.424542
	X1: -0.483466 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.423653
	X1: -0.482197 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.431581
	X1: -0.480995 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.431328
	X1: -0.479706 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.439879
	X1: -0.478483 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.440294
	X1: -0.47717 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.449523
	X1: -0.475922 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.450649
	X1: -0.47458 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.460617
	X1: -0.473303 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.462507
	X1: -0.471929 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.473284
	X1: -0.470619 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.476001
	X1: -0.469207 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.487673
	X1: -0.467859 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.491294
	X1: -0.466405 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.503956
	X1: -0.465015 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.508573
	X1: -0.463512 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.522338
	X1: -0.462073 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.528062
	X1: -0.460516 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.543063
	X1: -0.459023 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.550027
	X1: -0.457405 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.566416
	X1: -0.45585 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.57478
	X1: -0.454163 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.592741
	X1: -0.452538 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.602694
	X1: -0.450773 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.622442
	X1: -0.449071 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.634216
	X1: -0.447218 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.656006
	X1: -0.445427 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.669881
	X1: -0.443475 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.69402
	X1: -0.441584 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.710336
	X1: -0.43952 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.737191
	X1: -0.437515 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.756365
	X1: -0.435323 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.786384
	X1: -0.433189 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.80893
	X1: -0.430852 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.842659
	X1: -0.428571 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.869216
	X1: -0.426068 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.907326
	X1: -0.423618 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.938694
	X1: -0.420924 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 0.982022
	X1: -0.418279 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 1.01921
	X1: -0.415364 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 1.06881
	X1: -0.412493 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 1.11312
	X1: -0.409322 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 1.17031
	X1: -0.406189 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 1.22341
	X1: -0.402718 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 1.28992
	X1: -0.399276 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 1.354
	X1: -0.395452 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 1.43207
	X1: -0.391644 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	energia total: 1.51003
	X1: -0.387401 Y1: 0.938807
	X2: 0.97416 Y2: 0.928932
	
	
- Gráfico:

![grafico mola 1](https://github.com/gregsloap/TP1/blob/master/sprng.png)

- gráfico produzido com MathWorks Octave-like Online, segue o link: http://octave-online.net/;





### 3.0. Springmass 

### 3.1. Introdução: 
Essa Terceira parte do trabalho objetiva implementar métodos que descrevem o percurso da mola, agora com duas massas em seus extremos.

### 3.2 Pré-Requisitos: 

- Para a realização dessa etapa do trabalho foram necessarias as bibliotecas a seguir:
		
		iostream 
		springmass (contém a classe massa e classe mola, também usado na etapa anterior)
		simulation (contém a classe abstrata simulation)
		
- A versão do compilador utilizada foi gcc 4.9.2.
- Linhas de compilacao dos arquivos:

		cd < diretório > 

		g++ springmass.cpp test-springmass.cpp

## 3.3. Descrição dos arquivos:

- **springmass.h:** Define a Classe springmass seus métodos e atributos a serem utilizados na criação dos objetos .

	**Atributos de spring:** Coeficiente de amortecimento da mola, bem como seu Comprimento(deformação), Rigidez(resistencia a deformacao), as Massas a serem adicionadas em suas ponta, bem como a energia aplicada sobre si e sua força; 

	**Métodos de spring:** 

		Step: Calcula o passo da mola. 
		
		Display: Imprime os valores de saída.
		
- **springmass.cpp:** Contem as coordenadas da mola e a implementaçao dos metodos para "movimentá-la" e mantém registro de sua posição.
- **test-springmass.cpp:** Cria-se o Objeto e são executados os metodos da classe springmass, dando movimento de fato a mola.

### 3.4. Diagrama: 

![diagrama de classes](https://github.com/gregsloap/TP1/blob/master/diagramadeclasses2.png)

### 3.5. Saída de ***springmass*** :
*energia total acumulada, e as posições x1,y1,x2,y2 das massas, respectivamente.

		(-0.499722,0.0991)(0.499722,0.0991)$0.999444
		(-0.499077,0.0964)(0.499077,0.0964)$0.998154
		(-0.49832,0.0919)(0.49832,0.0919)$0.99664
		(-0.497541,0.0856)(0.497541,0.0856)$0.995082
		(-0.496772,0.0775)(0.496772,0.0775)$0.993543
		(-0.496023,0.0676)(0.496023,0.0676)$0.992046
		(-0.495298,0.0559)(0.495298,0.0559)$0.990596
		(-0.494597,0.0424)(0.494597,0.0424)$0.989194
		(-0.49392,0.0271)(0.49392,0.0271)$0.98784
		(-0.493266,0.01)(0.493266,0.01)$0.986533
		(-0.492635,-0.0089)(0.492635,-0.0089)$0.985271
		(-0.492026,-0.0296)(0.492026,-0.0296)$0.984052
		(-0.491438,-0.0521)(0.491438,-0.0521)$0.982876
		(-0.49087,-0.0764)(0.49087,-0.0764)$0.98174
		(-0.490322,-0.1025)(0.490322,-0.1025)$0.980644
		(-0.489792,-0.1304)(0.489792,-0.1304)$0.979585
		(-0.489281,-0.1601)(0.489281,-0.1601)$0.978563
		(-0.488788,-0.1916)(0.488788,-0.1916)$0.977576
		(-0.488312,-0.2249)(0.488312,-0.2249)$0.976623
		(-0.487852,-0.26)(0.487852,-0.26)$0.975704
		(-0.487408,-0.2969)(0.487408,-0.2969)$0.974816
		(-0.486979,-0.3356)(0.486979,-0.3356)$0.973958
		(-0.486565,-0.3761)(0.486565,-0.3761)$0.973131
		(-0.486166,-0.4184)(0.486166,-0.4184)$0.972331
		(-0.48578,-0.4625)(0.48578,-0.4625)$0.97156
		(-0.485408,-0.5084)(0.485408,-0.5084)$0.970815
		(-0.485048,-0.5561)(0.485048,-0.5561)$0.970096
		(-0.484701,-0.6056)(0.484701,-0.6056)$0.969402
		(-0.484366,-0.6569)(0.484366,-0.6569)$0.968731
		(-0.484042,-0.71)(0.484042,-0.71)$0.968084
		(-0.48373,-0.7649)(0.48373,-0.7649)$0.967459
		(-0.483428,-0.8216)(0.483428,-0.8216)$0.966856
		(-0.483137,-0.8801)(0.483137,-0.8801)$0.966274
		(-0.482856,-0.9404)(0.482856,-0.9404)$0.965712
		(-0.482584,-0.9404)(0.482584,-0.9404)$0.965169
		(-0.482322,-0.8801)(0.482322,-0.8801)$0.964645
		(-0.482069,-0.8216)(0.482069,-0.8216)$0.964139
		(-0.481825,-0.7649)(0.481825,-0.7649)$0.96365
		(-0.481589,-0.71)(0.481589,-0.71)$0.963179
		(-0.481362,-0.6569)(0.481362,-0.6569)$0.962724
		(-0.481142,-0.6056)(0.481142,-0.6056)$0.962284
		(-0.48093,-0.5561)(0.48093,-0.5561)$0.96186
		(-0.480725,-0.5084)(0.480725,-0.5084)$0.96145
		(-0.480527,-0.4625)(0.480527,-0.4625)$0.961054
		(-0.480336,-0.4184)(0.480336,-0.4184)$0.960672
		(-0.480152,-0.3761)(0.480152,-0.3761)$0.960304
		(-0.479974,-0.3356)(0.479974,-0.3356)$0.959948
		(-0.479802,-0.2969)(0.479802,-0.2969)$0.959604
		(-0.479636,-0.26)(0.479636,-0.26)$0.959272
		(-0.479476,-0.2249)(0.479476,-0.2249)$0.958952
		(-0.479321,-0.1916)(0.479321,-0.1916)$0.958643
		(-0.479172,-0.1601)(0.479172,-0.1601)$0.958344
		(-0.479028,-0.1304)(0.479028,-0.1304)$0.958056
		(-0.478889,-0.1025)(0.478889,-0.1025)$0.957777
		(-0.478754,-0.0764)(0.478754,-0.0764)$0.957509
		(-0.478625,-0.0521)(0.478625,-0.0521)$0.957249
		(-0.478499,-0.0296)(0.478499,-0.0296)$0.956999
		(-0.478379,-0.0089)(0.478379,-0.0089)$0.956757
		(-0.478262,0.01)(0.478262,0.01)$0.956524
		(-0.478149,0.0271)(0.478149,0.0271)$0.956298
		(-0.47804,0.0424)(0.47804,0.0424)$0.956081
		(-0.477935,0.0559)(0.477935,0.0559)$0.955871
		(-0.477834,0.0676)(0.477834,0.0676)$0.955668
		(-0.477736,0.0775)(0.477736,0.0775)$0.955472
		(-0.477641,0.0856)(0.477641,0.0856)$0.955283
		(-0.47755,0.0919)(0.47755,0.0919)$0.9551
		(-0.477462,0.0964)(0.477462,0.0964)$0.954924
		(-0.477377,0.0991)(0.477377,0.0991)$0.954754
		(-0.477295,0.1)(0.477295,0.1)$0.95459
		(-0.477216,0.0991)(0.477216,0.0991)$0.954431
		(-0.477139,0.0964)(0.477139,0.0964)$0.954278
		(-0.477065,0.0919)(0.477065,0.0919)$0.95413
		(-0.476994,0.0856)(0.476994,0.0856)$0.953988
		(-0.476925,0.0775)(0.476925,0.0775)$0.95385
		(-0.476858,0.0676)(0.476858,0.0676)$0.953717
		(-0.476794,0.0559)(0.476794,0.0559)$0.953589
		(-0.476732,0.0424)(0.476732,0.0424)$0.953465
		(-0.476672,0.0271)(0.476672,0.0271)$0.953345
		(-0.476615,0.01)(0.476615,0.01)$0.953229
		(-0.476559,-0.0089)(0.476559,-0.0089)$0.953118
		(-0.476505,-0.0296)(0.476505,-0.0296)$0.95301
		(-0.476453,-0.0521)(0.476453,-0.0521)$0.952906
		(-0.476403,-0.0764)(0.476403,-0.0764)$0.952806
		(-0.476354,-0.1025)(0.476354,-0.1025)$0.952709
		(-0.476308,-0.1304)(0.476308,-0.1304)$0.952615
		(-0.476262,-0.1601)(0.476262,-0.1601)$0.952525
		(-0.476219,-0.1916)(0.476219,-0.1916)$0.952438
		(-0.476177,-0.2249)(0.476177,-0.2249)$0.952353
		(-0.476136,-0.26)(0.476136,-0.26)$0.952272
		(-0.476097,-0.2969)(0.476097,-0.2969)$0.952194
		(-0.476059,-0.3356)(0.476059,-0.3356)$0.952118
		(-0.476022,-0.3761)(0.476022,-0.3761)$0.952045
		(-0.475987,-0.4184)(0.475987,-0.4184)$0.951974
		(-0.475953,-0.4625)(0.475953,-0.4625)$0.951906
		(-0.47592,-0.5084)(0.47592,-0.5084)$0.95184
		(-0.475888,-0.5561)(0.475888,-0.5561)$0.951776
		(-0.475857,-0.6056)(0.475857,-0.6056)$0.951715
		(-0.475828,-0.6569)(0.475828,-0.6569)$0.951656
		(-0.475799,-0.71)(0.475799,-0.71)$0.951599
		(-0.475772,-0.7649)(0.475772,-0.7649)$0.951543
- Grafico: 		
![diagrama de classes](https://github.com/gregsloap/TP1/blob/master/springmain.png)
