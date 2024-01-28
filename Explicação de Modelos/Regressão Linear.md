# Explicação do Modelo de Regressão Linear

## Introdução

Antes de entender sobre o modelo de regressão linear é necessário compreender sobre o `least square method` ou método dos mínimos quadrados. Este método é utilizado para encontrar a melhor reta que se ajusta aos dados. A reta é encontrada minimizando a soma dos quadrados das distâncias entre os pontos e a reta.

Esse método estatistico é o metodo que originou o modelo de regressão linear. Este modelo é utilizado para prever valores de uma variável contínua, além disso é uma técnica de aprendizado supervisionado.

## Least Square Method (Método dos Mínimos Quadrados)

A príncipio pode parecer complicado, mas na verdade é bem simples.

Vamos iniciar com um exemplo prático.

Imagine que você tenha $X$, uma lista com valores, mas vamos limita-lo para 5 pontos, ou seja, $X = [0,1,2,3,4]$

Agora vamos definir um valor para $Y$. $Y$ nada mais é do que uma função de $X$, ou seja, $Y = f(X)$.

Vamos supor que $Y$ tem os seguintes valores $Y = [-1, 3, 7, 11, 15]$.

A principio uma coisa importante de se observar é, não há ruído, ou seja os valores não possuem alguma variação, eles são exatos.

### Como encontrar a melhor reta que se ajusta aos dados?

Para isso é utilizado o `metodo dos minimos quadrados`. Vamos lá. Construiremos uma tabela para facilitar.

Para esse método, precisa-se dos valores de $X$, $Y$, $X^2$, $Y^2$ e $XY$.

Sabe-se que $X$ são valores distribuidos em um intervalo de 0 a 4, ou seja, $X = [0,1,2,3,4]$.

Sabe-se também que $Y$ é uma função de $X$, ou seja, $Y = f(X)$, logo $Y = [-1, 3, 7, 11, 15]$.

Observe que para cada valor de $X$ temos um valor de $Y$.

Agora vamos calcular $X^2$, $Y^2$ e $XY$.

$X^2 = [0, 1, 4, 9, 16]$

$Y^2 = [1, 9, 49, 121, 225]$

$XY = [0, 3, 14, 33, 60]$

Agora vamos construir uma tabela com os valores de $X$, $Y$, $X^2$, $Y^2$ e $XY$.

| X | Y | X^2 | Y^2 | XY |
|---|---|-----|-----|----|
| 0 | -1| 0   | 1   | 0  |
| 1 | 3 | 1   | 9   | 3  |
| 2 | 7 | 4   | 49  | 14 |
| 3 | 11| 9   | 121 | 33 |
| 4 | 15| 16  | 225 | 60 |

Com esses valores fica extremamente fácil encontrar a melhor reta que se ajusta aos dados.

Vamos lembrar da equação da reta:

$y = mx + b$

Onde $m$ é o coeficiente angular e $b$ é o coeficiente linear.

Para encontrar $m$ e $b$ é necessário utilizar as seguintes fórmulas:

$m = \frac{n\sum{xy} - \sum{x}\sum{y}}{n\sum{x^2} - (\sum{x})^2}$

$b = \frac{\sum{y} - m\sum{x}}{n}$

Onde $n$ é o número de pontos, ou seja, $n = 5$.

Próximo passo é obter o somatório de cada variável.

$\sum{x} = 10$

$\sum{y} = 35$

$\sum{x^2} = 30$

$\sum{y^2} = 405$

$\sum{xy} = 110$

Agora vamos substituir os valores na fórmula de $m$.

$m = \frac{5*110 - 10*35}{5*30 - 10^2}$

$m = \frac{550 - 350}{150 - 100}$

$m = \frac{200}{50}$

$m = 4$

Agora vamos substituir os valores na fórmula de $b$.

$b = \frac{35 - 4*10}{5}$

$b = \frac{35 - 40}{5}$

$b = \frac{-5}{5}$

$b = -1$

Agora que temos os valores de $m$ e $b$ podemos construir a equação da reta.

$y = 4x - 1$

Basicamente é dessa forma que o método dos mínimos quadrados funciona.

Vamos validar esse modelo.

Vamos tentar descobrir o valor de $y$ para $x = 3$

$y = 4*3 - 1$

$y = 12 - 1$

$y = 11$

O valor de $y$ para $x = 3$ é $11$.

O mesmo valor que temos na tabela.

Além disso pode ser feita uma predição para qualquer valor de $x$.

É claro é evidente que para esse exemplo tera valores exatos, pois não há ruído.

Além disso temos o coeficiente do modelo, que é dado por $R^2$.

$R^2 = \frac{\sum{(\hat{y} - \bar{y})^2}}{\sum{(y - \bar{y})^2}}$

Onde $\hat{y}$ é o valor predito, $y$ é o valor real e $\bar{y}$ é a média dos valores de $y$.

$R^2$ é um valor entre 0 e 1, quanto mais próximo de 1, melhor o modelo.

Vamos calcular o $R^2$ para o nosso exemplo.

Primeiro vamos calcular $\bar{y}$.

$\bar{y} = \frac{1}{5} * 35$

Onde $35$ é o somatório de $y$. e $5$ é o número de pontos.

$\bar{y} = 7$

Agora vamos calcular $\hat{y}$.

$\hat{y} = 4x - 1$

$\hat{y} = 4*0 - 1$

$\hat{y} = -1$

$\hat{y} = 4*1 - 1$

$\hat{y} = 3$

$\hat{y} = 4*2 - 1$

$\hat{y} = 7$

$\hat{y} = 4*3 - 1$

$\hat{y} = 11$

$\hat{y} = 4*4 - 1$

$\hat{y} = 15$

Agora vamos calcular $R^2$.

$R^2 = \frac{(3 - 7)^2 + (7 - 7)^2 + (11 - 7)^2 + (15 - 7)^2}{(-1 - 7)^2 + (3 - 7)^2 + (7 - 7)^2 + (11 - 7)^2 + (15 - 7)^2}$

$R^2 = \frac{16 + 0 + 16 + 64}{64 + 16 + 0 + 16 + 64}$

$R^2 = \frac{96}{176}$

$R^2 = 0.545$

O valor de $R^2$ é $0.545$.

Vamos verificar um exemplo com ruído.

Imagine a seguinte tabela:

|X | y | xy | x^2|
|---|---|---|---|
| 1 | 1.5 | 1.5 | 1 |
| 2 | 3.8 | 7.6 | 4 |
| 3 | 6.7 | 20.1 | 9 |
| 4 | 9 | 36 | 16 |
| 5 | 11.2 | 56 | 25 |
| 6 | 13.6 | 81.6 | 36 |
| 7 | 16 | 112 | 49 |

| $\sum X$ | $\sum y$ | $\sum xy$ | $\sum x^2$ |
|---|---|---|---|
| 28 | 61.8 | 315.8 | 140 |

Nesse caso, temos 7 pontos, ou seja, $n = 7$.

Agora vamos calcular $m$.

$m = \frac{7*315.8 - 28*61.8}{7*140 - 28^2}$

$m = \frac{2200.6 - 1718.4}{980 - 784}$

$m = \frac{482.2}{196}$

$m = 2.41$

Nesse caso, já é notável que o valor de $m$ não é mais inteiro.

Agora vamos calcular $b$.

$b = \frac{61.8 - 2.41*28}{7}$

$b = \frac{61.8 - 67.48}{7}$

$b = \frac{-5.68}{7}$

$b = -0.81$

Agora vamos construir a equação da reta.

$y = 2.41x - 0.81$

Fica nitido nesse caso que temos um ruído, pois os valores de $y$ não são exatos.

Caso substituirmos para validar esse modelo, encontraremos uma aproximação.

$y = 2.41*3 - 0.81$

$y = 7.23 - 0.81$

$y = 6.42$

O valor de $y$ para $x = 3$ é $6.42$.

O valor real é $6.7$.

## Regressão Linear

Agora que já entendemos o método dos mínimos quadrados, podemos entender o modelo de regressão linear.

A regressão linear é um modelo de aprendizado supervisionado, ou seja, é necessário ter os valores de $X$ e $Y$.

Os valores de $X$ será as features e os valores de $Y$ será o target.

No caso de um modelo teremos $n$ features e $1$ target. Onde $n$ features representaram $n$ coeficientes.

A equação da regressão linear é dada por:

$y = \beta_0 + \beta_1x_1 + \beta_2x_2 + ... + \beta_nx_n$

Onde $\beta_0$ é o coeficiente linear e $\beta_1, \beta_2, ..., \beta_n$ são os coeficientes angulares.

Para encontrar os coeficientes é necessário utilizar o método dos mínimos quadrados.

Para isso é necessário construir uma matriz $X$ e um vetor $Y$.

A matriz $X$ é dada por:

$X = \begin{bmatrix}
1 & x_{11} & x_{12} & ... & x_{1n} \\
1 & x_{21} & x_{22} & ... & x_{2n} \\
1 & x_{31} & x_{32} & ... & x_{3n} \\
... & ... & ... & ... & ... \\
1 & x_{m1} & x_{m2} & ... & x_{mn} \\
\end{bmatrix}$

Onde $m$ é o número de pontos e $n$ é o número de features.

O vetor $Y$ é dado por:

$Y = \begin{bmatrix}
y_1 \\
y_2 \\
y_3 \\
... \\
y_m \\
\end{bmatrix}$

Vamos supor alguns coeficientes:

Definindo alguns coeficientes:

$\beta_0 = -1.33470103e-01$

$\beta_1 = 3.58089136e-02$

$\beta_2 = 4.95226452e-02$

$\beta_3 = 3.11983512e+00$

$\beta_4 = -1.54170609e+01$

$\beta_5 = 4.05719923e+00$

$\beta_6 = -1.08208352e-02$

$\beta_7 = -1.38599824e+00$

$\beta_8 = 2.42727340e-01$

$\beta_9 = -8.70223437e-03$

$\beta_{10} = -9.10685208e-01$

$\beta_{11} = 1.17941159e-02$

$\beta_{12} = -5.47113313e-01$

Esses coeficientes foram obtidos utilizando o método dos mínimos quadrados.

Agora caso queira prever um valor, basta substituir na equação da regressão linear.

$y = -1.33470103e-01 + 3.58089136e-02x_1 + 4.95226452e-02x_2 + 3.11983512e+00x_3 -1.54170609e+01x_4 + 4.05719923e+00x_5 -1.08208352e-02x_6 -1.38599824e+00x_7 + 2.42727340e-01x_8 -8.70223437e-03x_9 -9.10685208e-01x_{10} + 1.17941159e-02x_{11} -5.47113313e-01x_{12}$

Vamos fazer um teste. 

Considere os seguintes valores para $x_1, x_2, ..., x_{12}$:

$x_1 = 0.00632$

$x_2 = 18.0$

$x_3 = 2.31$

$x_4 = 0$

$x_5 = 0.538$

$x_6 = 6.575$

$x_7 = 65.2$

$x_8 = 4.0900$

$x_9 = 1$

$x_{10} = 296.0$

$x_{11} = 15.3$

$x_{12} = 396.90$

Agora vamos substituir na equação da regressão linear.

$y = -1.33470103e-01 + 3.58089136e-02*0.00632 + 4.95226452e-02*18.0 + 3.11983512e+00*2.31 -1.54170609e+01*0.538 + 4.05719923e+00*6.575 -1.08208352e-02*65.2 -1.38599824e+00*4.0900 + 2.42727340e-01*1 -8.70223437e-03*296.0 -9.10685208e-01*15.3 + 1.17941159e-02*396.90 -5.47113313e-01*1$

Encotraremos o seguinte valor para $y$:

$y = 29.102$

![Imagem](/images/reglinear.png)

Quase encontramos o valor para o dataset de Boston.

## Mais informações

Algumas outras informações podem ser encontradas em outros repositorios meus.

Alguns repositorios que valem a pena dar uma olhada:

- [Regressão Linear](https://github.com/pcmoraesmenezes/Data-Science-and-Machine-Learning-Course/blob/main/Machine%20Learning%20Crash/practice/model_/linear_regression.ipynb)

Aqui, além de aplicação prática de um modelo de regressão linear usando o `scikit-learn`, também tem uma visualização do modelo. Vale a pena caso consida entender inglês.

- [Machine Learning](https://github.com/pcmoraesmenezes/Inteligencia-Artificial/blob/main/Livros/Machine%20Learning%20-%20Guia%20de%20Refer%C3%AAncia%20R%C3%A1pida/README.md)

Já esse outro repositorio é extremamente interessante para quem quer entender mais sobre Machine Learning. Ele é um guia de referência rápida, onde tem uma explicação sobre diversos modelos de Machine Learning. Esse repositorio é umas anotações sobre o livro `Machine Learning - Guia de Referência Rápida`. Além disso nesse repositorio tem varias outras coisas interessantes sobre Machine Learning e IA.

