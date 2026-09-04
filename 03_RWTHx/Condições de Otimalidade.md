Testes locais para mínimo irrestrito suave ($\Omega=\mathbb{R}^n$). Valem **num ponto**, não “para todo o espaço”.

## Ideia Central
- **Necessária** descarta: se falha, não é mínimo. **Suficiente** confirma: se vale, é mínimo. No caso geral, não temos as duas numa só.
- **1ª ordem (necessária):** mínimo local ⇒ $\nabla f(x^*)=0$.
- **2ª ordem (necessária):** mínimo local ⇒ $H(x^*)$ semidefinida positiva.
- **2ª ordem (suficiente):** estacionário + $H$ definida positiva ⇒ mínimo local *estrito*.
- $x^4$ é mínimo com $H=0$ (suficiente falha). $x^3$ e $-x^4$ cumprem a necessária e não são mínimos.
- Inclusões: suficientes ⊂ mínimos locais ⊂ 2ª necessária ⊂ 1ª necessária ⊂ $\mathbb{R}^n$.

## Exemplo
$f(x)=(x_2-x_1^2)(x_2-4x_1^2)$. Em $0$: $\nabla f=0$, $H$ PSD — necessárias ok, suficientes não. Mínimo em toda reta; na curva $x_2=2x_1^2$, $f=-2x_1^4$ — não é mínimo local.

## Quando
- **Usar:** classificar candidatos depois de achar estacionários.
- **Evitar:** parar no $\nabla f=0$ — pode ser máximo ou sela.

## Conexões
- [[Ponto Estacionário]]
- [[Gradiente]]
- [[Hessiana]]
- [[Solução Ótima]]
- [[Problema Convexo]]
- [[Conjunto Factível]]
