O número de escolhas livres do otimizador: as variáveis de decisão $x$ que as igualdades não fixam. A dimensão desse $x$ é a dimensão do espaço de busca.

## Ideia Central
Três papéis distintos, fácil misturar:

- **Decisão** ($x$) — o solver mexe (espessura de isolante, posição de uma turbina, vazão no tempo).
- **Parâmetro** — dado fixo (preço da energia, vento médio). Não entra em $x$.
- **Estado** — determinado pelas igualdades do modelo quando $x$ está fixo (temperatura que o balanço energético impõe).

Intuição: $n_{\mathrm{DOF}} \approx n_{\text{variáveis}} - n_{\text{igualdades independentes}}$. Cada igualdade independente “gasta” um grau de liberdade.

Mais DOF = mais flexibilidade **e** busca mais cara. A parametrização *é* a escolha de DOF: descrever uma forma por 3 números é um problema; deixar a geometria livre é outro (em tese, infinitos DOF até discretizar).

## Conexões
- [[Problema de Otimização]]
- [[Restrição]]
- [[Função Objetivo]]
- [[Solução Ótima]]
- [[Conjunto Factível]]
