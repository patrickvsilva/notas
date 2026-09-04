Formulação matemática do “melhor possível”: escolher [[Graus de Liberdade|variáveis de decisão]] que otimizam uma [[Função Objetivo]], respeitando [[Restrição|restrições]]. Sem isso, “ótimo” é opinião — melhoria intuitiva ou heurística, não garantia.

## Ideia Central
Quatro ingredientes:

1. **Variáveis** $x$ — o que se pode escolher ([[Graus de Liberdade]]).
2. **Função objetivo** $f$ — o número a minimizar ou maximizar.
3. **Modelo** — igualdades que descrevem o sistema (balanços, física).
4. **Restrições extras** — capacidades, qualidade, recursos, limites de $x$.

Forma canônica: minimizar $f(x)$ sujeito a $c_i(x)=0$ (igualdades) e $c_i(x)\le 0$ (desigualdades). Os pontos que cumprem tudo formam o [[Conjunto Factível]]. A [[Solução Ótima]] é o melhor factível — em geral um **compromisso** (ex.: mais isolamento reduz custo de aquecimento e aumenta investimento).

O **tipo** do problema (LP, NLP, inteiro, dinâmico, incerto) escolhe o algoritmo, não o contrário — [[Classificação de Problemas de Otimização]].

**Maldição do otimizador:** algoritmo bom + modelo ruim parece ótimo. Erro aleatório no modelo faz o valor *real* de $f$ ser pior do que o calculado; se o modelo permite ponto não-físico com $f$ boa, o solver vai escolhê-lo.

## Exemplo
Tubulação a $600^\circ\mathrm{C}$: o calor perdido exige aquecimento extra. Isolar reduz essa perda (custo operacional) e custa investimento. O DOF é a espessura do isolante; $f$ é o custo total anualizado.

## Quando
- **Usar:** critério mensurável e alternativas reais (projeto, operação, alocação).
- **Evitar:** objetivo vago ou modelo que mente mais do que ajuda — ótimo inútil.

## Conexões
- [[Função Objetivo]]
- [[Graus de Liberdade]]
- [[Restrição]]
- [[Solução Ótima]]
- [[Conjunto Factível]]
- [[Classificação de Problemas de Otimização]]
- [[Análise de Trade-offs]]
- [[Otimização Matemática para Engenheiros]]
