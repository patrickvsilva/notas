Propriedade geométrica de conjuntos e de funções. Um conjunto convexo não tem recortes: o segmento entre dois pontos fica dentro. Uma função convexa é “tigela”: a *corda* entre dois pontos fica acima do gráfico (a função fica abaixo da corda). É o que separa problema bem-comportado de problema com mínimos locais enganosos.

## Ideia Central
**Conjunto** $\Omega\subseteq\mathbb{R}^n$ é convexo se, para quaisquer $x_1,x_2\in\Omega$ e $\alpha\in[0,1]$, o ponto $\alpha x_1+(1-\alpha)x_2$ ainda está em $\Omega$. O segmento não sai. Não existe “conjunto côncavo” — ou é convexo, ou não é.

**Função** $f$ (em $D$ convexo) é convexa se

$$f(\alpha x_1+(1-\alpha)x_2)\le \alpha f(x_1)+(1-\alpha)f(x_2)$$

Estritamente convexa: a desigualdade é $<$ para $\alpha\in(0,1)$ (tigela sem trechos planos). Côncava = $-f$ convexa. Função afim (linear + constante) é convexa *e* côncava, mas não estrita.

Com $f$ suave: convexa ⇔ [[Hessiana]] semidefinida positiva em todo $D$; Hessiana definida positiva em todo $D$ ⇒ estritamente convexa.

O que isso muda no ótimo está em [[Problema Convexo]].

## Conexões
- [[Problema Convexo]]
- [[Hessiana]]
- [[Conjunto Factível]]
- [[Condições de Otimalidade]]
- [[Solução Ótima]]
