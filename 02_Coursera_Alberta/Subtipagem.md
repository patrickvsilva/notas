Relação entre tipos: um **subtipo** é utilizável onde o **supertipo** é esperado, porque o objeto do subtipo também “é” daquele tipo e comporta-se de acordo.

## Ideia
- Classe denota um **tipo** (o que os objetos podem fazer via métodos públicos).
- Ex: `Dog` subtipo de `Animal` → um dog é dog-typed **e** animal-typed (“um dog *é um* animal”).
- Em Java, subtipagem via:
  - [[Herança de Implementação]] (`extends`) — herda implementação; ou
  - [[Interface]] (`implements`) — cumpre o contrato, fornecendo os corpos.

Em ambos, um `Dog` pode ser usado onde o programa espera o tipo animal.

## Quando
- **Usar:** quando o subtipo pode substituir o supertipo em qualquer uso esperado ([[Princípio de Substituição de Liskov]]).
- **Evitar:** se o subtipo quebra o contrato do supertipo.

## Conexões
- [[Princípio de Substituição de Liskov]]
- [[Interface]]
- [[Herança]]
- [[Polimorfismo]]
- [[Generalização]]
