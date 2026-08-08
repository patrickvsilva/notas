Princípio: cada módulo revela o **mínimo** necessário para ser usado corretamente e **esconde** o resto. Outros módulos só acessam o que precisam para fazer o próprio trabalho.

## Regra de Ouro
| Revele (via interface) | Esconda |
|---|---|
| Premissas estáveis — o contrato em que outros podem confiar | Detalhes que **podem mudar** (implementação, estruturas internas) |

Ex: `String.concat(...)` — você usa a assinatura; não depende de como a concatenação é feita por baixo.

## Relação com [[Encapsulamento]]
- Ocultação de informação = a **ideia** (controle de acesso à informação).
- Encapsulamento = o **meio prático** (agrupar + interface + restringir), tipicamente com [[Modificadores de Acesso]] / [[Visibilidade UML]].
- Efeito: dá para mudar a implementação sem mudar o resultado esperado ([[Pensamento de Caixa Preta]], [[Barreira de Abstração]]).

## Também vale para atributos
Dados críticos ao comportamento da classe não devem ser alteráveis direto de fora — só por canais aprovados ([[Getters e Setters]]).

## Quando
- **Usar:** para revelar só o contrato estável e esconder o que pode mudar.
- **Evitar:** expor detalhes internos de que outros módulos passam a depender.

## Conexões
- [[Encapsulamento]]
- [[Modificadores de Acesso]]
- [[Visibilidade UML]]
- [[Interface]]
- [[Pensamento de Caixa Preta]]
- [[Barreira de Abstração]]
- [[Separação de Preocupações]]
- [[Modularidade]]
- [[Design Orientado a Objetos]]
