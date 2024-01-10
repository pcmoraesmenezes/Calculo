# Limite 🔣

## Introdução 📚

O conceito de limite de uma função $f$ é uma das ideias fundamentais do cálculo. Ele é tratado de forma intuitiva, ou seja supondo que $f(x)$ tende a um certo numero $L$ quando $x$ tende a um certo numero $a$. Quanto mais próximo de $a$ for $x$, mais próximo de $L$ será $f(x)$.

O limite fornece um meio de distinção de algumas funções com variação contínua e o comportamento de outras funções que variam independente das variaveis. A aplicação geométrica por trás do limite é o que conceitua a derivada e a integral.

### Notação 📝

$\lim_{x \to a} f(x) = L$ O limite de $f(x)$ quando $x$ tende a $a$ é igual a $L$.

### Exemplo 📐

Suponha que $f(x)$ é $x^2$ e que $x$ tende a $2$. Então, o limite de $f(x)$ quando $x$ tende a $2$ é igual a $4$.


#### Como calcular o limite? 🤔

Para calcular o limite de uma função $f(x)$ quando $x$ tende a $a$, basta substituir $x$ por $a$ na função $f(x)$.

$\lim_{x \to 2} x^2 = 4$

### Outros exemplos 📐

$\lim_ {x \to 3} 2x+5$

$\lim_ {x \to 3} 2x+5 = 2 \cdot 3 + 5 = 11$

Observe que até agora foi possível realizar o passo indutitvo, ou seja, realizar a substituição de $x$ por $a$ na função $f(x)$. Todavia nem sempre isso é possível, podendo acontecer de a função não estar definida no ponto $a$.

$\lim_ {x\to 2} \frac{2x² - 3x - 2}{x-2}$

Realizando a substituição de $x$ por $2$ na função $f(x)$, temos:

$\lim_ {x\to 2} \frac{2x² - 3x - 2}{x-2} = \frac{2 \cdot 2² - 3 \cdot 2 - 2}{2-2} = \frac{0}{0}$

Observe que a função não está definida no ponto $2$, pois o denominador é igual a $0$. Nesse caso, é necessário realizar uma simplificação algébrica para que seja possível realizar a substituição de $x$ por $2$ na função $f(x)$.

$\lim_ {x\to 2} \frac{2x² - 3x - 2}{x-2} = \lim_ {x\to 2} \frac{(2x+1)(x-2)}{x-2} = \lim_ {x\to 2} 2x+1 = 2 \cdot 2 + 1 = 5$

Gráfico da função $f(x) = \frac{2x² - 3x - 2}{x-2}$

![Gráfico da função f(x) = 2x² - 3x - 2/x-2](/images/1.png)

Observe que o comportamento da função $f(x)$ é diferente de $2x+5$, pois $f(x)$ não está definida no ponto $2$, mas o limite de $f(x)$ quando $x$ tende a $2$ é igual a $5$.

Observe que nesse caso o $lim_{x\to a}$ de $f(x)$ não é igual a $f(a)$, pois $f(a)$ não está definida.

Quando isso acontece, dizemos que $f(x)$ é uma função descontínua no ponto $a$.

### Exemplo 📐

$\lim_{x\to 2} 2x+1$

$\lim_{x\to 2} 2x+1 = 2 \cdot 2 + 1 = 5$

O gráfico gerado será uma reta sem furos ou saltos.

![Gráfico da função f(x) = 2x+1](/images/2.png)

## Definição formal de limite 🪄

Seja uma função $f$ definida em um intervalo aberto que contém o ponto $a$, exceto, possívelmente, o ponto $a$, e seja $l$ um numero ∈ R. Diz-se que o limite de $f(x)$ quando $x$ se aproxima de $a$ é $l$ e escreve-se:

$\lim_{x\to a} f(x) = l$

Isso implica que existe um erro definido como $\epsilon > 0$, ou seja um numero real arbitrariamente pequeno. Além disso existe uma diferença definida como $\delta > 0$, um numero suficientemente pequeno que 

se $0 < |x-a| < \delta$, então $|f(x) - l| < \epsilon$

Com isso tem-se:

1. $0 < |x-a| < \delta$ <=> $a - \delta < x < a + \delta$ e $x \neq a$

2. $|f(x) - l| < \epsilon$ <=> $l - \epsilon < f(x) < l + \epsilon$

![Gráfico](/images/3.png)

### Aplicação ✨

Dado $\epsilon = 0,02$, determine um $\delta > 0$ tal que, se $0 < |x-2| < \delta$, então $|(2x-1) -3| < \epsilon$.

Para isso tem-se que $(2x-1)$ é a função $f(x)$ e $3$ é o limite $l$.

$|(2x-1) -3| < \epsilon$

$|2x-4| < \epsilon$

$2|x-2| < \epsilon$

$|x-2| < \frac{\epsilon}{2}$

$|x-2| < \frac{0,02}{2}$

$|x-2| < 0,01$

$0 < |x-2| < 0,01$

$0 < x-2 < 0,01$

$2 < x < 2,01$

$\delta = 0,01$


### Retomando a definição formal de limite 🪄