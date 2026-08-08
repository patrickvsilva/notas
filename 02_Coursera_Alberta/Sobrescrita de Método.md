A subclasse fornece sua **própria implementação** de um método herdado da superclasse, substituindo o comportamento padrão sem mudar a assinatura do contrato.

## Ideia
- O método existe na superclasse; a subclasse redefine o *como*.
- Ex: `Animal.walk()` imprime “walking”; `Dog.walk()` imprime que prefere o sofá.

## No Código
| | Java |
|---|---|
| Marca | `@Override` (recomendado) |
| Ainda pode chamar o original | `super.walk()` |

## Quando
- **Usar:** especializar o *como* de um método herdado **sem** mudar o contrato do tipo base ([[Princípio de Substituição de Liskov]]).
- **Evitar:** sobrescrever para anular ou distorcer o significado esperado (ex: `walk()` que na verdade só nada).

## Conexões
- [[Herança]]
- [[Princípio de Substituição de Liskov]]
- [[Generalização]]
- [[Pensamento de Caixa Preta]]
- [[Princípio da Menor Surpresa]]
