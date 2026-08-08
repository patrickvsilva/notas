Princípio que exige: uma **subclasse** só pode substituir a **superclasse** se **não alterar** o comportamento esperado do tipo base — quem usa o supertipo continua correto ao receber o subtipo ([[Subtipagem]]).

## Ideia Central
- Se o código espera um `Animal`, um `Whale` passado no lugar deve continuar se comportando como animal *naquele contrato*.
- [[Sobrescrita de Método]] que troca o significado do método (ex: `walk()`/`run()` viram “nada a ver” / só nadar) **quebra** o princípio.

## Exemplo (violação)
`Animal` declara `eat`, `walk`, `run`. `Whale` sobrescreve `walk`/`run` com comportamento de natação → quem chama `animal.run()` não obtém o que o contrato de `Animal` promete.

## Quando
- **Usar (como teste):** antes de herdar, pergunte se a subclasse pode aparecer em todo lugar onde a superclasse é esperada, sem surpresas.
- **Evitar herança** se precisar anular ou distorcer comportamentos da superclasse — remodele ([[Decomposição]], hierarquia mais estreita, ou [[Interface]] específica).

## Conexões
- [[Herança]]
- [[Subtipagem]]
- [[Sobrescrita de Método]]
- [[Generalização]]
- [[Princípio da Menor Surpresa]]
- [[Decomposição]]
