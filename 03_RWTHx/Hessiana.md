A matriz das derivadas segundas de $f$. Captura a **curvatura**: se $f$ sobe, desce ou muda de sinal ao redor de um ponto. É o objeto da condição de 2ª ordem.

## Ideia Central
Se $f$ é $C^2$ (duas vezes continuamente diferenciável), $H(x)=\nabla^2 f(x)$ é simétrica, com $H_{ij}=\partial^2 f/\partial x_i\partial x_j$.

A forma quadrática $p^T H(x) p$ diz o que acontece na direção $p$:

- **Definida positiva** (autovalores $>0$): curvatura para cima em *toda* direção. Tigela.
- **Semidefinida positiva** (autovalores $\ge 0$): não desce, mas pode ser plana em alguma direção.
- **Indefinida** (autovalores com sinais mistos): sobe numa direção e desce em outra → sela.
- **Definida negativa** (autovalores $<0$): tigela invertida — candidato a máximo.

Isso liga duas notas: $H$ semidefinida positiva **em todo** $D$ ⇔ $f$ convexa ([[Convexidade]]); $H(x^*)$ no candidato entra nas [[Condições de Otimalidade]].

## Conexões
- [[Gradiente]]
- [[Convexidade]]
- [[Condições de Otimalidade]]
- [[Ponto Estacionário]]
- [[Função Objetivo]]
