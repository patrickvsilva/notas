Condição que um ponto precisa satisfazer para ser factível. Corta o espaço de busca: fora dela, a solução é inválida mesmo que $f$ esteja ótima.

## Ideia Central
Dois tipos:

- **Igualdade** $h(x)=0$ — o modelo do sistema (balanços, geometria). Consome [[Graus de Liberdade]].
- **Desigualdade** $g(x)\le 0$ — limites: capacidade, segurança, qualidade, disponibilidade de recurso, bounds de $x$.

Junto com o conjunto hospedeiro $D$ (onde $f$ e as $c_i$ estão definidas), formam o [[Conjunto Factível]] $\Omega$.

No ótimo, uma desigualdade está **ativa** se vale como igualdade ($g(x^*)=0$) e “segura” o ponto na fronteira; **inativa** se $g(x^*)<0$ e não aperta. Muitos ótimos de engenharia caem na fronteira — daí o trade-off entre solução boa e solução robusta (folga nas restrições).

Sem restrição extra, qualquer $x\in D$ é factível — caso irrestrito. Com restrição, o ótimo muitas vezes cai na fronteira.

## Quando
- **Usar:** limite físico, de segurança, de recurso ou de contrato que o ótimo não pode violar.
- **Evitar:** restrição inventada que esconde o verdadeiro objetivo — empurra o ótimo para o lugar errado.

## Conexões
- [[Problema de Otimização]]
- [[Graus de Liberdade]]
- [[Função Objetivo]]
- [[Conjunto Factível]]
- [[Solução Ótima]]
