Tipo de [[Herança]] em que a subclasse herda a **implementação** (atributos e métodos) de uma superclasse — em Java, via `extends`.

## Restrição (Java)
- **Herança simples:** uma subclasse → no máximo **uma** superclasse.
- Uma superclasse → **várias** subclasses (ex: `Dog` e `Cat` estendem `Animal`).
- A subclasse pode ela mesma ser superclasse de outra (herança em cadeia).

Para múltiplos tipos sem herdar implementação de várias classes: [[Interface]] (`implements`) — ver [[Herança Múltipla]].

## Quando
- **Usar:** subclasses compartilham estado/código concreto via `extends`, com *é-um* e [[Princípio de Substituição de Liskov]].
- **Evitar:** só contrato compartilhado ([[Interface]]); ou subclasse sem especialização própria.

## Conexões
- [[Herança]]
- [[Princípio de Substituição de Liskov]]
- [[Interface]]
- [[Herança Múltipla]]
- [[Generalização]]
- [[Classe Abstrata]]
- [[Subtipagem]]
