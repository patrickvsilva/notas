Ponto $x^*$ do [[Conjunto Factível]] com o melhor valor da [[Função Objetivo]]. É o que o [[Problema de Otimização]] procura — e pode não existir.

## Ideia Central
Três noções, da mais fraca à mais forte:

- **Mínimo local:** existe uma vizinhança $N(x^*)$ tal que $f(x^*)\le f(x)$ para todo factível nessa vizinhança. “Melhor aqui perto.”
- **Mínimo local estrito:** a desigualdade é estrita ($<$) para todo outro ponto da vizinhança. Não há platô.
- **Mínimo global:** $f(x^*)\le f(x)$ para **todo** $x\in\Omega$. “Melhor em qualquer lugar factível.”

Todo global é local. O contrário só vale em [[Problema Convexo]] (e casos triviais). $x^*$ pode estar no interior ou na fronteira de $\Omega$ — **nunca** fora (aí não é factível).

Pode não existir: $\Omega$ vazio (infactível) ou $f$ ilimitada por baixo. Métodos locais (descida, Newton, SQP) encontram um local e param; em problema não convexo isso não é o global.

Para *checar* um candidato no irrestrito suave, ver [[Condições de Otimalidade]].

## Conexões
- [[Problema de Otimização]]
- [[Função Objetivo]]
- [[Restrição]]
- [[Conjunto Factível]]
- [[Condições de Otimalidade]]
- [[Problema Convexo]]
- [[Eficiência de Algoritmos]]
