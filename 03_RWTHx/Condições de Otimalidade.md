Critérios matemáticos para decidir se um ponto candidato é mínimo local. No irrestrito suave usam o [[Gradiente]] (1ª ordem) e a [[Hessiana]] (2ª ordem): testam **aquele ponto**, não descrevem $f$ no espaço inteiro.

## Ideia Central
O solver devolve um candidato. As condições respondem: “esse ponto pode / deve ser mínimo?”. Há dois tipos de teste:

- **Necessária:** se $x^*$ é mínimo, a condição vale. Contrapositiva: se a condição *falha*, $x^*$ **não** é mínimo. Passar no teste não prova que é mínimo.
- **Suficiente:** se a condição vale, $x^*$ **é** mínimo. Falhar não prova nada — o ponto ainda pode ser mínimo.

No irrestrito ($\Omega=\mathbb{R}^n$), $f$ duas vezes continuamente diferenciável:

1. **1ª ordem (necessária):** mínimo local ⇒ $\nabla f(x^*)=0$. Ou seja, $x^*$ é [[Ponto Estacionário]]. Também vale em máximos e selas.
2. **2ª ordem (necessária):** mínimo local ⇒ $H(x^*)$ semidefinida positiva (curvatura não desce em direção nenhuma). Elimina *alguns* máximos e selas, não todos.
3. **2ª ordem (suficiente):** estacionário **e** $H(x^*)$ definida positiva ⇒ mínimo local *estrito* (num entorno, qualquer outro ponto é pior).

No caso geral **não** há um teste que seja necessário e suficiente ao mesmo tempo:

- $f(x)=x^4$ tem mínimo em $0$ com $H(0)=0$ — a suficiente falha, mas o ponto é mínimo.
- $f(x)=x^3$ e $f(x)=-x^4$ cumprem as necessárias em $0$ e não são mínimos.

Em [[Problema Convexo]], a 1ª ordem vira as duas coisas: estacionário ⇔ mínimo global.

## Exemplo
$f(x)=(x_2-x_1^2)(x_2-4x_1^2)$ em $0$: $\nabla f=0$ e $H$ semidefinida positiva — necessárias ok, suficiente não. Ao longo de qualquer *reta* por $0$, o ponto parece mínimo; na curva $x_2=2x_1^2$, $f=-2x_1^4$. Logo $0$ não é mínimo local de $f$.

## Quando
- **Usar:** depois de achar estacionários, para classificar (mínimo, máximo, sela, inconclusivo).
- **Evitar:** tratar $\nabla f=0$ como “achei o ótimo”.

## Conexões
- [[Ponto Estacionário]]
- [[Gradiente]]
- [[Hessiana]]
- [[Solução Ótima]]
- [[Problema Convexo]]
- [[Conjunto Factível]]
