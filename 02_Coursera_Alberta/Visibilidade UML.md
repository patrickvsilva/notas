Notação no [[Diagrama de Classes]] que indica quem pode acessar um atributo ou operação — expressão visual do [[Encapsulamento]] (e, com `#`, do acesso às subclasses na [[Herança]]).

## Símbolos
| Símbolo | Acesso | Significado |
|---|---|---|
| `+` | público | Acessível de fora da classe |
| `-` | privado | Acessível só de dentro da classe |
| `#` | protegido | Classe + **subclasses** (+ mesmo pacote, em Java) |

## No Código
| UML | Java | Python |
|---|---|---|
| `+` | `public` | sem underscore (público por padrão) |
| `-` | `private` | `_nome` forte / convenção de privado |
| `#` | `protected` | `_nome` (convenção; subclasses “podem” usar) |

## Conexões
- [[Diagrama de Classes]]
- [[Encapsulamento]]
- [[Herança]]
- [[Getters e Setters]]
- [[UML]]
