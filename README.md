 # Laboratório de Técnicas de programação 1.
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


### 1.4. Diagrama de Classes: 

![diagrama de classes]()


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
