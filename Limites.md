# Limite 🔣

## Tabela de conteúdos 📚

- [Introdução 📚](#introdução-📚)
    - [Notação 📝](#notação-📝)
    - [Exemplo 📐](#exemplo-📐)
        - [Como calcular o limite? 🤔](#como-calcular-o-limite-🤔)
        - [Outros exemplos 📐](#outros-exemplos-📐)
        - [Exemplo 📐](#exemplo-f09f9390-1)
            - [Aplicação ✨](#aplicação-✨)
            - [Retomando a definição formal de limite 🪄](#retomando-a-definição-formal-de-limite-🪄)
            - [Unicidade do limite 📐](#unicidade-do-limite-📐)
                - [Prova 📝](#prova-📝)
- [Limites laterais 📐](#limites-laterais-📐)
    - [A esquerda ⬅️](#a-esquerda-⬅️)
    - [A direita ➡️](#a-direita-➡️)
    - [Exemplo 📐](#exemplo-f09f9390-2)
    - [Existência do limite 📐](#existência-do-limite-📐)
    - [Exemplo 📐](#exemplo-f09f9390-3)
- [Função contínua 🛹](#função-contínua-🛹)
    - [Definição 📝](#definição-📝)
    - [Exemplo 🛞](#exemplo-f09f9390-3)
    - [Propriedades 📝](#propriedades-📝)
        - [Consequências das propriedades 🧲](#consequências-das-propriedades-🧲)
- [Limite e Continuidade de funções trigonométricas 📐](#limite-e-continuidade-de-funções-trigonométricas-📐)
- [Propriedade operatória dos limites 📐](#propriedade-operatória-dos-limites-📐)
    - [Exemplos 🧲](#exemplos-🧲)
    - [Casos em que as propriedades operatórias dos limites não podem ser aplicadas 🔦](#casos-em-que-as-propriedades-operatórias-dos-limites-não-podem-ser-aplicadas-🔦)
- [Limites que envolvem infinito ♾️](#limites-que-envolvem-infinito-♾️)
    - [Pela direita ➡️](#pela-direita-➡️)
    - [Pela esquerda ⬅️](#pela-esquerda-⬅️)
    - [Propriedades 📝](#propriedades-📝)
- [Teorema do confronto 🤼](#teorema-do-confronto-🤼)
- [Limites fundamentais ✅](#limites-fundamentais-✅)
    - [Limite fundamental trigonométrico ⭕](#limite-fundamental-trigonométrico-⭕)
        - [Exemplos ✈️](#exemplos-✈️)
    - [Limite fundamental da Função Potência Exponencial 📈](#limite-fundamental-da-função-potência-exponencial-📈)
        - [Exemplos ✈️](#exemplos-✈️-1)
    - [Consequências do limite fundamental da Função Potência Exponencial 📈](#consequências-do-limite-fundamental-da-função-potência-exponencial-📈)
        - [Exemplos ✈️](#exemplos-✈️-2)
- [Assintotas 🪂](#assíntotas-📐)
    - [Assintotas horizontais 🪂](#assíntota-horizontal-🪂)
    - [Assintotas verticais 🪂](#assíntota-vertical-🪂)
        - [Exemplo 📐](#exemplo-f09f9390-5)
    - [Assintotas inclinadas 🪂](#assintota-inclinada-🪂)
        - [Exemplo 📚](#exemplo-📚)
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

Se para todo $\epsilon > 0$ existe um $\delta > 0$ tal que se $0 < |x-a| < \delta$, então $|f(x) - l| < \epsilon$, então $|f(x) - l| < \epsilon$.

$L$ é o limite se for possível fazer $f(x)$ se aproximar dele apenas fazendo com que o $x$ se aproxima de $a$. Isto deve ser válido para toda forma de aproximação possível.

$\epsilon$ e   $\delta$ tornam a ideia do aproximar menos vagas.

### Unicidade do limite 📐

Para a existência do limite, ele deve ser considerado com sendo único ou seja

$\lim_{x\to a} f(x) = l$ e $\lim_{x\to a} f(x) = l'$, então $l = l'$

#### Prova 📝

Considerando um erro aribtrário $\epsilon > 0$, como $lim_{x\to a} f(x) = l_{1}$, então existe uma diferença maior que 0, ou seja $\delta > 0$ tal que o modulo da diferença de $f(x)$ pelo valor do limite $l_{1}$ seja menor que o erro $\epsilon$. Isso ocorre sempre que o modulo da diferença de $x$ por $a$ é maior que 0 e é menor que a diferença. O inverso também é válido, ou seja para um $lim_{x\to a} f(x) = l_{2}$, existe uma diferença $\delta > 0$ tal que o modulo da diferença entre $f(x)$  e o $l_{2}$ é menor que um erro aceitavel $\epsilon$. Isso ocorre sempre que o modulo da diferença de $x$ por $a$ é maior que 0 e é menor que a diferença.

Dito isso escolhe-se o menor $\delta$ entre os dois, ou seja, $\delta = min(\delta_{1}, \delta_{2})$.

$|f(x) - l_{1}| < \frac{\epsilon}{2}$ e $|f(x) - l_{2}| < \frac{\epsilon}{2}$

Utilizando a propriedade da desigualdade triângular, ou seja $|a + b| \leq |a| + |b|$, tem-se:

$|l_{1} - l_{2}|$ = $|- f(x) + l_{1} + f(x) - l_{2}|$ $\gt$ $ - (|f(x) - l_{1}| + |f(x) - l_{2}|)$

$|-(f(x) - l_{1}) + (f(x) - l_{2})|$ $\gt$ $ - (|f(x) - l_{1}| + |f(x) - l_{2}|)$

$|f(x) - l_{2}| \lt \frac{\epsilon}{2} + \frac{\epsilon}{2}$

Como $\epsilon$ é arbitrário, então $|f(x) - l_{2}| \lt \epsilon$

## Limites laterais 📐

### A esquerda ⬅️

Diz-se que o limite se aproxima pela esquerda quando $x \lt a$. Nesse caso, o limite é escrito como $lim_{x\to a^{-}} f(x) = l$.

### A direita ➡️

Diz-se que o limite se aproxima pela direita quando $x \gt a$. Nesse caso, o limite é escrito como $lim_{x\to a^{+}} f(x) = l$.

### Exemplo 📐

Calcule $lim_{x\to 1^{-}} f(x) e lim_{x\to 1^{+}} f(x)$

$f(x) = x^{2}$, se $x \lt 1$

$f(x) = 3x$ se $x \gt 1$

$lim_{x\to 1^{-}} f(x) = lim_{x\to 1^{-}} x^{2} = 1$

$lim_{x\to 1^{+}} f(x) = lim_{x\to 1^{+}} 3x = 3$

Observe a imagem

![Gráfico da função f(x) = x² se x < 1 e f(x) = 3x se x > 1](/images/4.jpeg)

Pela teoria da unicidade dos limites pode se afirmar que os limites são diferentes, ou seja não existe o limite de $f(x)$ quando $x$ tende a $1$.

### Existência do limite 📐

$∃ lim_{x\to a} f(x)$ se e somente se $lim_{x\to a^{-}} f(x) = lim_{x\to a^{+}} f(x)$

### Exemplo 📐

$f(x) = x^{2}$, se $x \lt 2$

$f(x) = 1$, se $x = 2$

$f(x) = -x+6$, se $x \gt 2$

$lim_{x\to 2^{-}} f(x) = lim_{x\to 2^{-}} x^{2} = 4$

$lim_{x\to 2^{+}} f(x) = lim_{x\to 2^{+}} -x+6 = 4$

Existe o limite de $f(x)$ quando $x$ tende a $2$ e é igual a $4$.

## Função contínua 🛹

Conforme visto no exemplo anterior pode ocorrer do limite existir, mesmo se $f(x)$ não for definido em $a$; ou seja pode ocorrer de $f(x)$ estar definida em $a$ e existir o limite de $f(x)$ quando $x$ tende a $a$.

Quando $lim_{x\to a} f(x) = f(a)$, diz-se que $f(x)$ é contínua em $a$.

### Definição 📝

$f: [b, c] \to R$ é contínua em $a \in [b, c]$ se $lim_{x\to a} f(x) = f(a)$

$a \in [b, c]$, se:

- $f$ é definida no ponto $a$
- $lim_{x\to a} f(x)$ existe
- $lim_{x\to a} f(x) = f(a)$

### Exemplo 🛞

$f(x) = \frac{|x|}{x}$

$\frac{x}{x} = 1$, se $x \gt 0$

$\frac{-x}{x} = -1$, se $x \lt 0$

$lim_{x\to 0^{-}} f(x) = lim_{x\to 0^{-}} -1 = -1$

$lim_{x\to 0^{+}} f(x) = lim_{x\to 0^{+}} 1 = 1$

A função não é contínua em $0$, pois $lim_{x\to 0^{-}} f(x) \neq lim_{x\to 0^{+}} f(x)$

### Outro exemplo ⚙️

$f(x) = x^{2}$, se $x \lt 2$

$f(x) = 4$, se $x = 2$

$f(x) = -x+6$, se $x \gt 2$

$lim_{x\to 2^{-}} f(x) = lim_{x\to 2^{-}} x^{2} = 4$

$lim_{x\to 2^{+}} f(x) = lim_{x\to 2^{+}} -x+6 = 4$

$lim_{x\to 2} f(x) = lim_{x\to 2} f(x) = 4$

A função é contínua em $2$, pois $lim_{x\to 2} f(x) = f(2)$

### Propriedades 📝

Se $f$ e $g$ são contínuas em $a$, então:

1. $f + g$ é contínua em $a$

2. $f \cdot g$ é contínua em $a$

3. $\frac{f}{g}$ é contínua em $a$, se $g(a) \neq 0$

4. $f - g$ é contínua em $a$

#### Consequências das propriedades 🧲

Se $m$, $b$ e $a$ $\in R$, então:

1. $lim_{x\to a} mx+b = ma+b$

Se $f$ é uma função polinomial, então:

2. $lim_{x\to a} f(x) = lim_{x\to a} (b_{n}x^{n} + b_{n-1}x^{n-1} + ... + b_{1}x + b_{0}) = b_{n}a^{n} + b_{n-1}a^{n-1} + ... + b_{1}a + b_{0} = f(a)$

Se $lim_{x\to a} g(x) = b$ e $f$ é contínua em $b$, então:

3. $lim_{x\to a} f(g(x)) = f(lim_{x\to a} g(x)) = f(b)$

## Limite e Continuidade de funções trigonométricas 📐

1. $lim_{x\to a} sen(x) = sen(a)$

2. $lim_{x\to a} cos(x) = cos(a)$

3. $lim_{x\to a} tg(x) = tg(a)$ = $\frac{sen(x)}{cos(x)}$ = $\frac{sen(a)}{cos(a)}$

4. $lim_{x\to a} cotg(x) = cotg(a)$ = $\frac{cos(x)}{sen(x)}$ = $\frac{cos(a)}{sen(a)}$

5. $lim_{x\to a} sec(x) = sec(a)$ = $\frac{1}{cos(x)}$ = $\frac{1}{cos(a)}$

6. $lim_{x\to a} cossec(x) = cossec(a)$ = $\frac{1}{sen(x)}$ = $\frac{1}{sen(a)}$

## Propriedade operatória dos limites 📐

Se $f(x) = c$, tal que $f(x)$ é uma função constante, então $lim_{x\to a} f(x) = c$

Considere que: $lim_{x\to a} f(x) = l_{1}$ e $lim_{x\to a} g(x) = l_{2}$

1. $lim_{x\to a} (f(x) + g(x)) = lim_{x\to a} f(x) + lim_{x\to a} g(x) = l_{1} + l_{2}$

2. $lim_{x\to a} (f(x) - g(x)) = lim_{x\to a} f(x) - lim_{x\to a} g(x) = l_{1} - l_{2}$

3. $lim_{x\to a} (f(x) \cdot g(x)) = lim_{x\to a} f(x) \cdot lim_{x\to a} g(x) = l_{1} \cdot l_{2}$

4. $lim_{x\to a} \frac{f(x)}{g(x)} = \frac{lim_{x\to a} f(x)}{lim_{x\to a} g(x)} = \frac{l_{1}}{l_{2}}$, se $l_{2} \neq 0$

5. $lim_{x\to a} (f(x))^{n} = (lim_{x\to a} f(x))^{n} = l_{1}^{n}$

6. $lim_{x\to a} \sqrt[n]{f(x)} = \sqrt[n]{lim_{x\to a} f(x)} = \sqrt[n]{l_{1}}$, se $l_{1} \geq 0$

7. $lim_{x\to a} (f(x))^{g(x)} = (lim_{x\to a} f(x))^{lim_{x\to a} g(x)} = l_{1}^{l_{2}}$, se $l_{1} \gt 0$

8. $lim_{x\to a} c \cdot f(x) = c \cdot lim_{x\to a} f(x) = c \cdot l_{1}$

9. $lim_{x\to a} log_{c} f(x) = log_{c} lim_{x\to a} f(x) = log_{c} l_{1}$, se $l_{1} \gt 0$

### Exemplos 🧲

1. Dado $f(x) = 3$ Calcule $lim_{x\to 2} f(x)$

$lim_{x\to 2} f(x) = 3$

#### Calcule usando as propriedades operatorias dos limites:

2. $lim_{x\to 3} (5 - 2x + |x|)$

$lim_{x\to 3} (5 - 2x + |x|) = lim_{x\to 3} 5 - lim_{x\to 3} 2x + lim_{x\to 3} |x| = 5 - 2 \cdot 3 + |3| = 5 - 6 + 3 = 2$

3.  $lim_{x\to \frac{\pi}{6}} (sen(x) - cos(x))$

$lim_{x\to \frac{\pi}{6}} (sen(x) - cos(x)) = lim_{x\to \frac{\pi}{6}} sen(x) - lim_{x\to \frac{\pi}{6}} cos(x) = sen(\frac{\pi}{6}) - cos(\frac{\pi}{6}) = \frac{1}{2} - \frac{\sqrt{3}}{2} = \frac{1 - \sqrt{3}}{2}$

### Casos em que as propriedades operatórias dos limites não podem ser aplicadas 🔦

1. $lim_{x\to 3} \frac{x^{2} - 9}{x - 3}$

$lim_{x\to 3} \frac{x^{2} - 9}{x - 3} = lim_{x\to 3} \frac{(x - 3)(x + 3)}{x - 3} = lim_{x\to 3} x + 3 = 3 + 3 = 6$

Nesses casos devem ser selecionados os valores próximos de $3$, mas não iguais a $3$.

## Limites que envolvem infinito ♾️

### Pela direita ➡️

Seja $f$ uma função em um intervalo $]a;b[$, então:

$lim_{x\to a^{+}} f(x) = +\infty$ se para todo $M > 0$ existe um $\delta > 0$ tal que se $a < x < a + \delta$, então $f(x) > M$

Lembrando que $\infty$ não é simbolo de um numero, mas sim de uma ideia de crescimento sem limites.

### Pela esquerda ⬅️

Seja $f$ uma função em um intervalo $]a;b[$, então:

$lim_{x\to a^{-}} f(x) = -\infty$ se para todo $M < 0$ existe um $\delta > 0$ tal que se $a - \delta < x < a$, então $f(x) < M$

--- 
Se $f$ é uma função definida em ambos os lados de $a$ exceto em $a$, então:

$lim_{x\to a} f(x) = +\infty$ se para todo $M > 0$ existe um $\delta > 0$ tal que se $0 < |x - a| < \delta$, então $f(x) > M$

$lim_{x\to a} f(x) = -\infty$ se para todo $M < 0$ existe um $\delta > 0$ tal que se $0 < |x - a| < \delta$, então $f(x) < M$

Logo se $lim_{x\to a} f(x) = +\infty$, $f(x)$ pode ser arbitrariamente grande.

### Propriedades 📝

1. Se $lim_{x\to a} f(x) != 0 = l$ e $lim_{x\to a} g(x) = 0$, então $lim_{x\to a} \frac{f(x)}{g(x)} = \pm \infty$

2. $lim_{x\to +\infty} (\frac{1}{x})^{p}$ = 

$lim_{x\to +\infty} \frac{1}{x^{p}}$ = $0$, se $p > 0$

3. $lim_{x\to a} P(x) = lim_{x\to +\infty} a_{m}x^{m}$ e $lim_{x\to +\infty} a_{n}x^{n}$ =

$+\infty$, se $m > n$

$0$, se $m < n$

$\frac{a_{m}}{a_{n}}$, se $m = n$

## Teorema do confronto 🤼

Seja $I$ um intervalo aberto, onde existe $f$, $g$ e $h$ definidas em $I$ exceto, possivelmente, em $a$ e $lim_{x\to a} f(x) = lim_{x\to a} h(x) = l$ e $f(x) \leq g(x) \leq h(x)$, para todo $x \in I$, então $lim_{x\to a} g(x) = l$

Usando a definição formal de limite, tem-se:

$lim_{x\to a} f(x) = l$ e $lim_{x\to a} h(x) = l$, então:

$\forall \epsilon > 0, \exists \delta_{1} > 0$ tal que se $0 < |x - a| < \delta_{1}$, então $|f(x) - l| < \epsilon$

$\forall \epsilon > 0, \exists \delta_{2} > 0$ tal que se $0 < |x - a| < \delta_{2}$, então $|h(x) - l| < \epsilon$

Escolhendo $\delta = min(\delta_{1}, \delta_{2})$, tem-se:

$0 < |x - a| < \delta$, então $|f(x) - l| < \epsilon$ e $|h(x) - l| < \epsilon$

Como $f(x) \leq g(x) \leq h(x)$, então $|f(x) - l| \leq |g(x) - l| \leq |h(x) - l|$

Logo $|g(x) - l| < \epsilon$

O teorema do confronto é utilizado para calcular limites que não podem ser calculados diretamente. Esses limites dão origem aos limites fundamentais.

## Limites fundamentais ✅

### Limite fundamental trigonométrico ⭕

$lim_{x\to 0} \frac{sen(x)}{x} = 1$

Mas por que $lim_{x\to 0} \frac{sen(x)}{x} = 1$? 🤔

![Gráfico da função f(x) = sen(x)/x](/images/5.png)

Seja o arco $AOP$, $x in ]0; \frac{\pi}{2}[$, então:

$sen(x) < x < tg(x)$

$tg(x) = \frac{sen(x)}{cos(x)}$

Como $sen(x) > 0$ então é possível aplicar uma multiplicação em função de $sen(x)$, ou seja:

$\frac{sen(x)}{sen(x)} > \frac{sen(x)}{x} > \frac{sen(x)}{tg(x)}$

$1 > \frac{sen(x)}{x} > cos(x)$

Aplicando limite em ambos os lados da desigualdade, tem-se:

$lim_{x\to 0} 1 = 1$ > $lim_{x\to 0} \frac{sen(x)}{x}$ > $lim_{x\to 0} cos(x) = 1$

Logo $lim_{x\to 0} \frac{sen(x)}{x} = 1$

#### Exemplos ✈️

1. $lim_{x\to 0} \frac{sen(3x)}{x}$

$lim_{x\to 0} \frac{sen(3x)}{x} = 3 \cdot lim_{x\to 0} \frac{sen(3x)}{3x} = 3 \cdot 1 = 3$

2. $lim_{x\to 0} \frac{sen(2x)}{5x}$

$lim_{x\to 0} \frac{sen(2x)}{5x} = \frac{1}{5} \cdot lim_{x\to 0} \frac{sen(2x)}{2x}$

$\frac{1}{5} \cdot lim_{x\to 0} \frac{2\cdot sen(2x)}{2\cdot x}$

$\frac{1}{5} \cdot 2 \cdot lim_{x\to 0} \frac{sen(2x)}{2x}$

$\frac{2}{5} \cdot 1 = \frac{2}{5}$

### Limite fundamental da Função Potência Exponencial 📈

$lim_{x\to \infty} (1 + \frac{1}{x})^{x} = e$

Prova:

Considere $x$ = $\frac{1}{t}$, então $t$ = $\frac{1}{x}$

Sendo que $x->$ $o^{+}$, então $t$ = $\frac{1}{x}->$ $+\infty$

e $x->$ $0^{-}$, então $t$ = $\frac{1}{x}->$ $-\infty$

$lim_{x\to \infty} (1 + \frac{1}{x})^{x} = lim_{t\to 0^{+}} (1 + t)^{\frac{1}{t}} = e$

$lim_{x\to -\infty} (1 + \frac{1}{x})^{x} = lim_{t\to 0^{-}} (1 + t)^{\frac{1}{t}} = e$


#### Exemplos ✈️

1. $lim_{x\to \infty} (1 + \frac{1}{x})^{2x}$

$lim_{x\to \infty} (1 + \frac{1}{x})^{2x} = lim_{x\to \infty} ((1 + \frac{1}{x})^{x})^{2} = e^{2}$

2. $lim_{x\to \infty} (1 + \frac{1}{x})^{3x}$

$lim_{x\to \infty} (1 + \frac{1}{x})^{3x} = lim_{x\to \infty} ((1 + \frac{1}{x})^{x})^{3} = e^{3}$

3. $lim_{x\to \infty} (1 + \frac{5}{x})^{x}$

$lim_{x\to \infty} (1 + \frac{5}{x})^{x} = lim_{x\to \infty} ((1 + \frac{5}{x})^{\frac{x}{5}})^{5} = e^{5}$

### Consequências do limite fundamental da Função Potência Exponencial 📈

$lim_{x\to 0} \frac {a^{x} - 1}{x} = ln(a)$, se $a > 0$

Prova:

$a$ = 1 => $lim_{x\to 0} \frac {1^{x} - 1}{x} = lim_{x\to 0} \frac {0}{x} = 0$ = $ln(1)$

Se $0 < a != 1$, então $t = a^{x} - 1$ e $x = \frac{ln(1 + t)}{ln(a)}$

$lim_{x\to 0} \frac {a^{x} - 1}{x} = lim_{t\to 0} \frac {t}{\frac{ln(1 + t)}{ln(a)}} = lim_{t\to 0} \frac {t \cdot ln(a)}{ln(1 + t)} = ln(a) \cdot lim_{t\to 0} \frac {t}{ln(1 + t)} = ln(a)$

#### Exemplos ✈️

1. $lim_{x\to 0} \frac {2^{x} - 1}{x}$

$lim_{x\to 0} \frac {2^{x} - 1}{x} = ln(2)$

2. $lim_{x\to 0} \frac {2^{x+2} - 1}{x}$

$lim_{x\to 0} \frac {2^{x+2} - 1}{x} = lim_{x\to 0} \frac {2^{x} \cdot 2^{2} - 1}{x} = \frac{4}{3} \cdot ln(2)$

## Assíntotas 📐

### Assíntota horizontal 🪂

A reta $y = b$ é assíntota horizontal de $y = f(x)$ se uma das condições for satisfeita:

1. $lim_{x\to +\infty} f(x) = b$

2. $lim_{x\to -\infty} f(x) = b$

Ou seja é necessário que a função retorne um valor escalar constante.

### Assíntota vertical 🪂

A reta $x = a$ é assintota vertical de $y = f(x)$ se uma das condições for satisfeita:

1. $lim_{x\to a^{-}} f(x) = +\infty$ 

2.  $lim_{x\to a^{+}} f(x) = -\infty$

3. $lim_{x\to a^{-}} f(x) = -\infty$

4. $lim_{x\to a^{+}} f(x) = +\infty$

#### Exemplo 📐

$f(x) = \frac{3x-2}{x-2}$

Colocando o x em evidência no numerador e no denominador, tem-se:

$f(x) = \frac{x(3-\frac{2}{x})}{x(1-\frac{2}{x})}$

É possível simplificar os termos em evidência, pois $x \neq 0$:

$f(x) = \frac{3-\frac{2}{x}}{1-\frac{2}{x}}$

$f(x) = 3$

$lim_{x\to +\infty} f(x) = 3$

$lim_{x\to -\infty} f(x) = 3$

Para verificar se é assintota vertical

$lim_{x\to 2^{-}} f(x) = lim_{x\to 2^{-}} \frac{3-\frac{2}{x}}{1-\frac{2}{x}} = -\infty$

$lim_{x\to 2^{+}} f(x) = lim_{x\to 2^{+}} \frac{3-\frac{2}{x}}{1-\frac{2}{x}} = +\infty$

### Assintota Inclinada 🪂

A reta $y = mx + b$ é assintota inclinada de $y = f(x)$ se uma das condições for satisfeita:

1. $lim_{x\to +\infty} (f(x) - (mx + b)) = 0$

2. $lim_{x\to -\infty} (f(x) - (mx + b)) = 0$

Para ser assintota inclinada o grau da diferença entre o maior polinômio do numerador e o maior polinômio do denominador deve ser igual a $1$.

#### Exemplo 📚

Verificar se y = 3x é assintota

$f(x) = \frac{3x^{3} +4x}{x^{2} + 4}$

$lim_{x\to +\infty} (f(x) - (mx + b)) = 0$

$lim_{x\to +\infty} (\frac{3x^{3} +4x}{x^{2} + 4} - (mx + b)) = 0$

$lim_{x\to +\infty} (\frac{3x^{3} +4x}{x^{2} + 4} - (3x)) = 0$

$lim_{x\to +\infty} (\frac{3x^{3} +4x}{x^{2} + 4} - \frac{3x^{3} + 12}{x^{2} + 4}) = 0$

$lim_{x\to +\infty} \frac{3x{3} + 4x - 3x \dot(x^{2} + 4)}{x^{2} + 4}$

$lim_{x\to +\infty} \frac{-8x}{x^{2} + 4} = 0$
