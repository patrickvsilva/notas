Classe que generaliza um conceito mas **não pode ser instanciada** diretamente — só através de subclasses concretas. Expressa que o tipo é incompleto ou genérico demais para existir sozinho (ex: `Animal`).

## No Código
| | Java | Python |
|---|---|---|
| Declaração | `abstract class Animal` | `class Animal(ABC):` |
| Efeito | `new Animal()` é ilegal | instanciar `Animal()` falha se abstrata de fato |

Atributos e métodos concretos na abstrata ainda são herdados pelas subclasses ([[Herança]]). Como [[Interface]], é um meio de obter [[Polimorfismo]] (mesmo contrato, implementações nas subclasses).

## Interface vs classe abstrata (nesta trilha)
| | [[Classe Abstrata]] | [[Interface]] |
|---|---|---|
| Pode ter atributos / estado | sim | não (só comportamentos) |
| Pode ter implementação | sim (métodos concretos) | não (só assinaturas)* |
| Herança múltipla (Java) | não (`extends` um) | sim (`implements` vários) |

\*Em Java moderno há `default` methods; o curso trata a interface clássica (só contrato).

## Conexões
- [[Herança]]
- [[Interface]]
- [[Polimorfismo]]
- [[Generalização]]
- [[Abstração]]
- [[Diagrama de Classes]]
