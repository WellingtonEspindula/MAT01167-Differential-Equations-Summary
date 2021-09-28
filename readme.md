# Equações Diferenciais

## Por: Wellington Espindula

## Equações Diferenciais de primeira ordem:

$$y' = f(x, y)$$

### Equações a **variáveis separáveis:**

Diz-se que uma equação diferencial é a variáveis separáveis quando puder ser escrito sobre a forma 

$$y' = g(x) \cdot h(y)$$

**MÉTODO:**

- **Separar as variáveis**
- **Integrar** termo a termo

**Não-Homogêneas:**

A ideia é **fatorar** e a partir da fatoração fazer a separação de variáveis, integração, etc.

### Equações lineares de primeira ordem**:**

$$y' + P(x)y = Q(x)$$

**MÉTODO:**

Se $Q(x) = 0$, a equação é **linear homogênea**. Nesse caso, o **método já é conhecido**.

Caso contrário é **linear não-homogênea**.

- 1ª Etapa: **Resolução** da equação linear **homogênea associada** à equação dada

    $$y'+ P(x) = 0$$

    Só resolver a equação à **variáveis separáveis**

- 2ª Etapa: **Método da variação do parâmetro**

    Queremos determinar $C(x)$ tal que a abaixo seja solução da equação diferencial dada.

    $$y = C(x) e^{g(x)}$$

    - **Deriva-se $y$** e **substitui-se**  $y'$ na equação inicial
    - Resolvendo a equação, **encontra-se $C(x)$**
    - **Substitui $C(x)$** na resolução da **equação associada**.

### Equações diferenciais de Bernoulli**:**

$$\frac{dx}{dt} = f(t)x + g(t)x^{\alpha}$$

onde:

$$\alpha \neq \space \land \space \alpha \neq 1$$

**MÉTODO:**

- **Multiplica a equação por $x^{-α}$**

    $$x^{- \alpha}(\frac{dx}{dt}) = x^{- \alpha} ( f(t)x + g(T)x^{\alpha} )$$

- Faz-se uma **mudança de variável**
- **Deriva a nova variável** e **substitui** na equação
- **Resolve a equação diferencial** de primeira ordem encontrada

### Equações diferenciais exatas**:**

As equações diferenciais, sob a forma canônica abaixo, são exatas tais que exista uma função u(x, y), de modo que ela possa ser escrita como du = 0.

$$M(x, y)dx +N(x, y)dy = 0$$

- **1º Passo**: **Reescrever** a equação em sua **forma canônica**:

    $$3xy+y² + (x²+xy)y' = 0  \Rightarrow (x²+xy) \frac{dy}{dx} = - (3xy+y²)$$

    $$(x²+xy)dy= - (3xy+y²)dx \Rightarrow (3xy+y²)dx + (x²+xy)dy = 0$$

    Desse modo,

    $$M(x, y) = (3xy+y²)dx; \space N(x, y) = (x²+xy)dy $$

- **2º Passo: Verificar** se a equação **é exata**

    $$\frac{\partial M(x, y)}{\partial y} = \frac{\partial N(x, y)}{\partial x}$$

- **SE** a equação for **exata:**
    - A solução será simplesmente:

        $$u(x, y) = C \text{, isso decorre da premissa } du = 0$$

        **Determinação da função u(x, y):**

        $$du = \frac{\partial u}{\partial x} + \frac{\partial u}{\partial y}$$

        $$\frac{\partial u}{ \partial x} = M(x, y) \space \land \space \frac{\partial u}{ \partial y} = N(x,y)$$

        Tendo como exemplo:

        $$\textbf{(1) } \space M(x,y) = 2x+y²$$

        $$\textbf{(2) } \space N(x,y) = 2xy$$

        Para satisfazer a condução **(1)**:

        $$\textbf{(3) }\space u(x, y) = x^2 + xy + f(y)$$

        sendo **f(y)** uma função qualquer **APENAS** de **y**.

        Faz-se a **derivada parcial** de **(3)** agora em relação à **y** e **iguala-se à condição** **(2)**.

        $$\frac{\partial u}{\partial  y} = 2xy + \frac{df}{dy} \Rightarrow 2xy + \frac{df}{dy} = 2xy \Rightarrow \frac{df}{dy} = 0$$

        $$f(y) = C_1$$

        Portanto:

        $$u(x,y) = x^2 + xy^2 + C_1$$

        Logo, a solução geral será:

        $$u(x, y) = C \Rightarrow x^2 + xy^2 + C_1 = C$$

        Substituindo C1 e C por uma única constante essencial:

        $$x^2 + xy^2 = K$$

- **SE** a equação **NÃO** for **exata:**
    - **Determinação de um Fator Integrante:**
        - **Multiplica-se φ** por M e N

            $$\phi \cdot M(x,y) dx + \phi \cdot N(x,y) dy = 0$$

        - **Deriva-se e iguala**

            $$\frac{\partial \phi u}{\partial y} = \frac{\partial \phi u}{\partial x}$$

        - **Resolvendo,** encontramos:

            $$g(x) = \frac{\phi (\frac{\partial M}{\partial y} + \frac{\partial N}{\partial x})}{N}$$

        - Então:

            $$\phi (x) = e^{\int{g(x)dx}} \text{, onde }\phi (x) \text{ é fator integrante da equação dif dada}$$

    - **Tipo Especial (se existir)**

        $$\phi(x, y) = x^{\alpha} \cdot y^{\beta}$$

        - **Multiplica-se** a equação por x^α * y^β

            $$x^{\alpha} \cdot y^{\beta} (M(x,y)dx + N(x,y)dy) = 0$$

        - **Deriva-se e iguala**

            $$\frac{\partial \phi u}{\partial y} = \frac{\partial \phi u}{\partial x}$$

        - **Resolve-se o sistema** para α e β. **Se existir a solução** desse sistema, **existe o fator integrante**. Caso contrário, não existe.

## Equações Diferenciais de **ordem 2** (ou para ordens acima de 2):

$$\textbf{(1) }\space y'' + p(x)y' + q(x)y = b(x)$$

### Equações **homogêneas** à coeficientes **constantes (b(x) = 0):**

### Equação característica

$$1y''+ 2y'+3y = 0 \\
r'' +2r' +3r = 0 \\
r_1, r_2 = \frac{-b \pm \sqrt{b^2 -4ac}}{2a}$$

- **1º caso:  $r_1, \space r_2 \in  \real : r_1 \neq r_2$**

    **Solução Geral:**

    $$y = C_1 e^{r_1x} + C_1 e^{r_2x}$$

- **2º caso: $r_1, r_2 \not\in \real \space and \space r_1 \neq r_2$**

    $$r = c \pm di, d \neq 0$$

    **Solução Geral:**

    $$y = e^{cx} \cdot [C_1\cos(dx)+C_2\sin(dx)]$$

    ou também pode ser sob a forma:

    $$y = A \cos(dx - \delta)$$

  ****

- **3º caso: $r_1 = r_2$**

    **Solução Geral:**

    $$y = C_1 \cdot e^{rx} + C_2 \cdot  y_2(x)$$

    $$y_2(x) = u(x) \cdot y_1(x)$$

### Equações **não-homogêneas** à coeficientes **constantes (b(x) ≠ 0):**

$$\text {Solução geral: }\space y(x) = y_c(x) + y_p(x) $$

$$\text{onde }y_c \text{ é função complementar e } y_p \text{ é a solução particular}$$

- Método dos **coeficientes a determinar:**

$$\text{Só é possível se  }b(x) \text{ tiver os seguintes formatos:}$$

$$\text{(1) ... } e^{\alpha t} : Ae^{\alpha t} \text{, onde } A \text{ é um coeficiente a determinar}$$

$$\text{(2) ... } \sin(\beta t) \text{ e/ou ...} \cos(\beta t) : A \sin(\beta t) + B \cos(\beta t) \text{, onde A e B são coeficientes a determinar}$$

$$\text{(3) } ...t^{n} + ...t^{n-1} + ... + t^0 \text{ : }D_{1}t^{n} + D_{2}t^{n-1} + ... + D_{n}t + D_{n+1} \text{, onde }D_{1}, D_{2}, D_{...}, D_n \text{ e } D_{n+1} \text{ são coeficientes a determinar}$$

$$\text{(4) } ...e^{\alpha t}\sin{\beta t} \text{  e/ou  } ...e^{\alpha t}\cos{\beta t}  \text{ : } Ae^{\alpha t}\sin{\beta t} + Be^{\alpha t}\cos{\beta t} \text{, onde A e B são coeficientes a determinar}$$

$$\text{(5) } P_{n}(t)e^{\alpha t}\sin{\beta t} \text{  e/ou  } P_{n}(t)e^{\alpha t}\cos{\beta t} \text{ : }  (D_{1}t^{n} + D_{2}t^{n-1} + ... + D_{n}t + D_{n+1})e^{\alpha t}\sin{\beta t} + (E_{1}t^{n} + E_{2}t^{n-1} + ... + E_{n}t + E_{n+1})e^{\alpha t}\cos{\beta t})$$

**OBSERVAÇÃO:** Lembrar que no caso da solução particular é de **EXTREMA IMPORTÂNCIA** verificar em cada termo de **b(x)** a soma 

$$\alpha \pm \beta i$$

**SE** a soma acima for igual à(s) raiz(es) da Equação característica:

$$Ae^{2x} \cdot x^{s}$$

sendo **S** a multiplicidade da raiz.

- Método de **variação de parâmetros:**

    $$\text{Pode ser usada para todos os formatos de   }b(x)$$

    $$y_{p} = C_1(x) y_1(x) + C_2(x) y_2(x)$$

    - Substituímos o y(p) na equação diferencial **(1)**, bem como suas derivadas
    - Cortamos todos os termos que irão zerar (soluções da equação homogênea associada).

        $$y_1'' + p(x)y_1'+q(x)y_1 = 0$$

        $$y_2'' + p(x)y_2'+q(x)y_2 = 0$$

    - Impomos:

        $$\textbf{(2) } \space C_{1}' y_{1} + C_{2}' y_{2} = 0$$

    - Derivamos em relação à **x**

        $$\textbf{(3) } \space C_{1}' y_{1}' + C_{1}'' y_{1} + C_{2}' y_{2}' + C_{2}'' y_{2} = 0$$

    - Resolvamos o sistema formado por **(2)** e **(3)**

### Equações **homogêneas** à coeficientes **variáveis (b(x) = 0):**

### Cauchy-Euler

A equação de Cauchy-Euler é um **tipo especial** de equação diferenciais linear a **coeficientes variáveis** que pode ser resolvida sem usar o método de série de potências dado que admite uma mudança de variável adequada em que recai em outra equação diferencial à coeficientes consantes**:**

$$a_n x^n y ^{(n)} + a_{n-1} x^{n-1} y ^{(n-1)} + ... + a_2 x^2 y'' + a_1 x y' + a_0 y = b(x)$$

A equação de Cauchy-Euler **não precisa ser homogênea.**

**MÉTODO:**

- Faz-se a mudança na **variável independente**

    $$Z \equiv ln(x) \rightarrow x = e^z$$

- Faz a **derivada,** bem como a mudança de variáveis usando a regra da cadeia

    $$\frac{dy}{dx} = \frac{dy}{dz} \cdot \frac{dz}{dx} = \frac{dy}{dz} \cdot e^{-z}$$

    $$\frac{d^2y}{dx^2} = \frac{d(y')}{dz} \cdot \frac{dz}{dx} = \frac{d(y')}{dz} \cdot e^{-z} => \frac{d^2y}{dx²} = (e^{-z} \frac{d^2y}{dz^2} - e^{-z} \frac{dy}{dz}) \cdot e^{-z} => \frac{d^2y}{dx²} = (\frac{d^2y}{dz^2} - \frac{dy}{dz}) \cdot e^{-2z}$$

- Substitui-se **x** e as **derivadas de y** na equação original e obtemos algo do tipo:

    $$a_2 \frac{d^2y}{dz^2} + (-a_2 + a_1) \frac{dy}{dz} + a_0 y = 0$$

- **Resolvamos** a equação a **coeficientes constantes**
- Por fim, **substituímos z por x de volta**

### Método da Série de Potências:

$$y = \sum_{n=0}^{\infty}{A_n (x-x_0)^n}$$

**OBS.:** Geralmente, usa-se **x0 = 0**, dado que a série se ajustará melhor nos pontos radiais ao x = 0 quando for feita uma aproximação por truncamento da série.

$$y = \sum_{n=0}^{\infty}{A_n x^n}$$

**MÉTODO:**

- **Deriva-se** a série em relação à x, chegando em **y'** e **y''**

    $$y' = \sum_{n=1}^{\infty}{A_n (n) x^{n-1}}$$

    $$y'' = \sum_{n=2}^{\infty}{A_n (n)(n-1) x^{n-2}}$$

- **Substitui** na equação inicial **(1)**

    $$y'' + p(x)y' + q(x)y = 0$$

    $$\sum_{n=2}^{\infty}{A_n (n)(n-1) x^{n-2}} + p(x)\sum_{n=1}^{\infty}{A_n (n) x^{n-1}} + q(x)\sum_{n=0}^{\infty}{A_n x^n} = 0$$

- **Ajustam-se os expoentes**
- **Ajustam-se os índices** dos somatórios
- Com os termos que sobraram fora do somatório, **criam-se relações entre as constantes**
- Com os termos dentro do somatório, **criam-se a relação de recorrência** entre as constantes
- Com as relações de constantes, verifica-se se as relações entre as constantes inicialmente encontrada podem ser encontradas na relação de recorrência.

### Método de Frobenius:

$$y = \sum_{n=0}^{\infty}{C_n (x-x_0)^{n+r}}$$

O método de Froubenius é utilizado em uma equação 

$$y'' + p(x)y' + q(x)y = 0$$

tal que um ponto $**x_0$** (normalmente, $**x_0 = 0**$) é um **ponto singular regular.**

A fim de verificar se um ponto é singular regular, verificamos se as funções abaixo **F(x)** e **G(x)** são **analíticas em x = x0.**

$$F(x) = (x-x_0) \cdot p(x)$$

$$G(x) = (x-x_0)^2 \cdot q(x)$$

**MÉTODO:**

$$y = \sum_{n=0}^{\infty}{C_n \cdot x^{n+r}} \text{, tendo em vista } x_0 = 0$$

- **Deriva-se** a série em relação à x, chegando em **y'** e **y''. OBS.:** Aqui, no derivar, **não muda-se o índice do somatório.**

    $$y' = \sum_{n=0}^{\infty}{C_n (n+r) x^{n+r-1}}$$

    $$y'' = \sum_{n=0}^{\infty}{C_n (n+r)(n+r-1) x^{n+r-2}}$$

- **Substitui** na equação inicial **(1)**

    $$y'' + p(x)y' + q(x)y = 0$$

    $$\sum_{n=0}^{\infty}{C_n (n+r)(n+r-1) x^{n+r-2}} + p(x)\sum_{n=0}^{\infty}{C_n (n+r) x^{n+r-1}} + q(x)\sum_{n=0}^{\infty}{C_n x^{n+r}} = 0$$

- **Ajustam-se os expoentes**
- **Ajustam-se os índices** dos somatórios
- Com os termos que sobraram fora do somatório, **criam-se relações entre as constantes,** e, desse modo, obteremos, fatorando **r**, a **Equação Indicial.**

    $$\text{Por exemplo: } C_0(r^2+2r+1) = 0$$

- Com a equação indicial **encontraremos 2 possíveis valores de r**
- Com os termos dentro do somatório, **criam-se a relação de recorrência** entre as constantes
- Após isso, para cada caso de **r**, **veremos os valores de Cn** que a série gera.
- Com isso, cada valor de **r nos dará uma solução para a equação diferencial**
- Utilizando o **princípio de superposição de soluções**, encontramos a **solução geral da equação diferencial.**

## Série de Fourier:

$$g(x) = \sum_{m=0}^{\infty}{a_m \cos{\frac{m \pi x}{L}}} + \sum_{n=0}^{\infty}{B_n \cos{\frac{n \pi x}{L}}}$$

Afim de utilizarmos somente a parte que nos interessa na série de Fourier, fazemos considerações de **paridade** sobre a função escolhida, e, deste modo, se a função for par ou ímpar deixamos somente a parte do cosseno ou do seno conforme o que está abaixo:

$$\cos(x) \rightarrow \text{ função \textbf{par} } \rightarrow f(-x) = f(x) $$

$$\sin(x) \rightarrow \text{ função \textbf{ímpar}} \rightarrow f(-x) = - f(x)$$

Após as considerações de paridade, chegamos a g(x) com cosseno e/ou seno. Então, calcularemos os coeficientes $a_m$ e/ou $b_n$

**MÉTODO:**

- **Montar a g(x)**
    - Reconhecemos o conjunto ortogonal {...} no intervalo [-L,+L]
    - Considerações de **paridade**
- **Encontrar os coeficientes** da(s) série(s)

    $$\underset{m = 0,1, 2, ...}{a_m} = \frac{\int_{-L}^{+L} f(x) \cos(\frac{m \pi x}{L})dx}{\int_{-L}^{+L} \cos^2(\frac{m \pi x}{L})dx}$$

    $$\underset{n = 1,2, ...}{b_n} = \frac{\int_{-L}^{+L} f(x) \sin(\frac{m \pi x}{L})dx}{\int_{-L}^{+L} \sin^2(\frac{m \pi x}{L})dx}$$

    **OBS.:** No caso do $A_m$, é necessário **lembrar que tem que ser calculado $a_0$**

    $$a_0 = \frac{\int_{-L}^{+L} f(x) dx}{\int_{-L}^{+L}dx}$$

- **Resolver as integrais**
- Se necessário, fazer **observações de paridade** no resultado e, caso precise, **ajustar índices para excluir termos nulos**
- **Substituir coeficientes** e fazer os **ajustes dos índices** caso o tenha realizado no passo anterior

## Equações Diferenciais Parciais:

Equações diferencias que envolvem funções de duas ou mais variáveis.

### Método de Separação de Variáveis

- Equação da **Difusão do calor**

    $$\textbf{(1) }\space \frac{\partial^2u}{\partial x^2} = \frac{1}{\alpha^2} \frac{\partial u}{\partial t}$$

- Equação da **Onda unidimensional**

    $$\textbf{(2) }\space \frac{\partial^2u}{\partial x^2} = \frac{1}{v^2} \frac{\partial^2 u}{\partial t^2}$$

- Equação de **Laplace**

$$\nabla^2u = \frac{1}{\alpha^2} \frac{\partial u}{\partial t}$$

$$\nabla^2u = \frac{\partial^2u}{\partial x^2} = \frac{1}{v^2} \frac{\partial^2 u}{\partial t^2}$$

**MÉTODO** (Tomando **(1)** como exemplo)**:**

- **Separar as variáveis** (...óbvio)

    $$\textbf{(3) }\space u(x, t) = X(x) \cdot T(t)$$

- **Derivar a equação (3)** em relação à **x** e em relação à **t** quantas vezes o necessário a fim de substituir na equação original

    $$\frac{\partial^2 u}{\partial x^2} = X''T$$

    $$\frac{\partial u}{\partial t} = XT'$$

- **Substituir** na equação diferencial

    $$X''T = \frac{1}{\alpha ^2} XT'$$

- **Isolar as variáveis** e **igualar a uma constante**

    $$\frac{X''}{X} = \frac{T'}{\alpha T} = \lambda$$

- Resolver o **problema de contorno** relativo à **parte espacial**

    $$X'' - \lambda X = 0$$

    **OBS.:** Os **valores de contorno** serão retirados do **enunciado do problema** sob a forma similar à abaixo

    $$u(0, t) = 0 \Rightarrow X(0) = 0  \newline u(\pi) = 0 \Rightarrow X(\pi) = 0 $$

    No fim, deve-se **chegar a um valor de λn** (ou vn) e Xn(x)

- Resolver a **parte espacial**
- **Substituir Xn(x) e Tn(t)** em **(3):**

    $$u_n(x,t) = X_n(x) \cdot T_n(t)$$

- Aplica-se o **Princípio da superposição de soluções:**

    $$\textbf{(4) }\space u(x, t) = \sum_{n = }^{\infty} C_n X_n(x) T_n(t)$$

- Por fim, resolve-se o **problema de valor inicial**
    - Nesse passo, chegaremos a algo do tipo

        $$f(x) = \sum_{n=}^{\infty} C_n \sin(\frac{m\pi x}{L})$$

    - Então, resolveremos com **Série de Fourier** para encontrarmos Cn
- E então, **substituiremos a constante encontrada** em **(4)**