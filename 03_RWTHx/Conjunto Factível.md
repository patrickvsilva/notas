O conjunto $\Omega$ de todos os pontos que o [[Problema de Otimização]] aceita: estão no conjunto hospedeiro $D$ e satisfazem todas as [[Restrição|restrições]]. Uma [[Solução Ótima]] só pode existir aqui.

## Ideia Central
$D\subseteq\mathbb{R}^n$ é onde $f$ e as restrições estão definidas (muitas vezes uma caixa $x_{\min}\le x\le x_{\max}$, ou $\mathbb{R}^n$ inteiro). As restrições recortam $D$:

$$\Omega = \{ x \in D \mid c_i(x) \le 0\ \forall i \in I,\ c_i(x) = 0\ \forall i \in E \}$$

- $\Omega$ **vazio** → problema infactível (nenhuma escolha cumpre o modelo e os limites).
- $\Omega=\mathbb{R}^n$ → otimização irrestrita: qualquer $x$ é legal; só $f$ decide.
- O ótimo pode estar no **interior** de $\Omega$ (restrições de desigualdade folgadas) ou na **fronteira** (pelo menos uma ativa). Fora de $\Omega$ o ponto é inválido, por melhor que $f$ pareça.

A [[Convexidade]] de $\Omega$ muda teoria e algoritmo: conjunto convexo não tem “buracos” nem recortes côncavos.

## Conexões
- [[Restrição]]
- [[Solução Ótima]]
- [[Problema de Otimização]]
- [[Convexidade]]
- [[Graus de Liberdade]]
