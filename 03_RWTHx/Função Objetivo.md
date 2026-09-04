O critério numérico que o [[Problema de Otimização]] minimiza ou maximiza. Sem ela não há “melhor” — só o [[Conjunto Factível|factível]].

## Ideia Central
$f$ resume o que importa a um número: custo, lucro, tempo de ciclo, área, risco, throughput. Pode ser econômica, técnica ou uma mistura (custo anualizado = operação + investimento). Na tubulação, $f$ é esse custo total — não a espessura do isolante.

Maximizar $f$ é o mesmo que minimizar $-f$. A convenção dos livros é minimizar.

Vários critérios ao mesmo tempo (custo **e** qualidade) não cabem numa $f$ só. Duas saídas: ponderar numa combinação, ou transformar os outros em [[Restrição]] (“qualidade ≥ piso”) e otimizar um. É a versão formal da [[Análise de Trade-offs]].

O ótimo costuma ser compromisso: melhorar um efeito piora outro. $f$ precisa deixar esse conflito explícito — senão o solver “otimiza” o que você não quis.

## Conexões
- [[Problema de Otimização]]
- [[Restrição]]
- [[Solução Ótima]]
- [[Análise de Trade-offs]]
- [[Atributos de Qualidade]]
