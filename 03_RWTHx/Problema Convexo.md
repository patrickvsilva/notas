[[Problema de Otimização]] em que a [[Função Objetivo]] $f$ é convexa e o [[Conjunto Factível]] $\Omega$ é convexo. Aí todo mínimo local é global, e achar um [[Ponto Estacionário]] resolve o problema.

## Ideia Central
$\Omega$ fica convexo quando as desigualdades $c_i$ ($i\in I$) são convexas e as igualdades ($i\in E$) são **lineares**. Uma igualdade não linear em geral curva $\Omega$ e quebra a convexidade.

Por que local = global: convexidade impede $f$ de descer de novo depois de um vale. Se $x^*$ é mínimo local, não existe outro vale distinto.

Se $f$ é convexa e suave, a desigualdade $f(x)\ge f(x^*)+\nabla f(x^*)^T(x-x^*)$ vale para todo $x$. Com $\nabla f(x^*)=0$, isso vira $f(x)\ge f(x^*)$ em todo o espaço: estacionário ⇔ mínimo **global**. A 1ª ordem das [[Condições de Otimalidade]] deixa de ser só necessária — vira também suficiente.

Em restrito convexo vale o análogo (KKT necessária e suficiente — semanas seguintes).

## Quando
- **Usar:** reconhecer convexidade antes de resolver — o solver local já entrega o global.
- **Evitar:** tratar NLP não convexo como se o estacionário fosse o ótimo global.

## Conexões
- [[Convexidade]]
- [[Conjunto Factível]]
- [[Condições de Otimalidade]]
- [[Ponto Estacionário]]
- [[Classificação de Problemas de Otimização]]
- [[Solução Ótima]]
