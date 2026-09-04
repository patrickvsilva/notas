O vetor das derivadas parciais de $f$. Aponta a direção de **maior subida**; o oposto é a de maior descida. É o objeto da condição de 1ª ordem.

## Ideia Central
Para $f:\mathbb{R}^n\to\mathbb{R}$ diferenciável:

$$\nabla f(x) = \begin{pmatrix} \partial f/\partial x_1 \\ \vdots \\ \partial f/\partial x_n \end{pmatrix}$$

A **derivada direcional** na direção $p$ (o quanto $f$ muda ao dar um passo infinitesimal em $p$) coincide com o produto interno $\nabla f(x)^T p$. Por isso, se $\nabla f(x^*)\ne 0$, existe uma direção que *diminui* $f$ — $x^*$ não pode ser mínimo.

Se $\nabla f(x^*)=0$, não há direção de primeira ordem que desça: $x^*$ é [[Ponto Estacionário]]. Necessário para mínimo irrestrito suave; **não** suficiente (pode ser máximo ou sela). Ver [[Condições de Otimalidade]].

## Conexões
- [[Hessiana]]
- [[Ponto Estacionário]]
- [[Condições de Otimalidade]]
- [[Função Objetivo]]
- [[Solução Ótima]]
