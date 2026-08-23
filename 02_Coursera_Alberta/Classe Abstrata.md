Classe que generaliza um conceito mas **não pode ser instanciada** diretamente — só através de subclasses concretas. Expressa que o tipo é incompleto ou genérico demais para existir sozinho (ex: `Animal`).

## No Código
- Declaração: `abstract class Animal`
- Efeito: `new Animal()` é ilegal

## No UML
Nome da classe e da operação abstrata em *itálico*; sem itálico, `{abstract}` — ver [[Diagrama de Classes]].

Atributos e métodos concretos na abstrata ainda são herdados pelas subclasses ([[Herança]]). Como [[Interface]], é um meio de obter [[Polimorfismo]] (mesmo contrato, implementações nas subclasses).

## Interface vs classe abstrata (nesta trilha)
| | [[Classe Abstrata]] | [[Interface]] |
|---|---|---|
| Pode ter atributos / estado | sim | não (só comportamentos) |
| Pode ter implementação | sim (métodos concretos) | não (só assinaturas)* |
| Herança múltipla (Java) | não (`extends` um) | sim (`implements` vários) |

\*Em Java moderno há `default` methods; o curso trata a interface clássica (só contrato).

## Quando
- **Usar:** base parcial compartilhada que não deve ser instanciada sozinha.
- **Evitar:** se só há contrato sem implementação/estado — use [[Interface]].

## Conexões
- [[Herança]]
- [[Interface]]
- [[Polimorfismo]]
- [[Generalização]]
- [[Abstração]]
- [[Diagrama de Classes]]
