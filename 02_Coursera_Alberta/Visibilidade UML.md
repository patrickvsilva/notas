Notação no [[Diagrama de Classes]] que indica quem pode acessar um atributo ou operação — expressão visual de [[Ocultação de Informação]] / [[Encapsulamento]] (e, com `#`, do acesso às subclasses na [[Herança]]).

## Símbolos
| Símbolo | Acesso (Java) | Significado |
|---|---|---|
| `+` | `public` | Qualquer classe |
| `#` | `protected` | Classe + subclasses + mesmo pacote |
| `~` | default (sem modificador) | Só o mesmo pacote |
| `-` | `private` | Só a própria classe |

## No Código
| UML | Java | Python |
|---|---|---|
| `+` | `public` | `nome` |
| `#` | `protected` | `_nome` (convenção) |
| `~` | *(sem modificador)* | — (sem equivalente direto) |
| `-` | `private` | `_nome` / `__nome` |

Detalhe dos quatro níveis: [[Modificadores de Acesso]].

## Conexões
- [[Modificadores de Acesso]]
- [[Ocultação de Informação]]
- [[Diagrama de Classes]]
- [[Encapsulamento]]
- [[Herança]]
- [[Getters e Setters]]
- [[UML]]
