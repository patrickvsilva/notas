A subclasse fornece sua **própria implementação** de um método herdado da superclasse, substituindo o comportamento padrão sem mudar a assinatura do contrato.

## Ideia
- O método existe na superclasse; a subclasse redefine o *como*.
- Ex: `Animal.walk()` imprime “walking”; `Dog.walk()` imprime que prefere o sofá.

## No Código
| | Java | Python |
|---|---|---|
| Marca | `@Override` (recomendado) | redefinir o método com o mesmo nome |
| Ainda pode chamar o original | `super.walk()` | `super().walk()` |

## Conexões
- [[Herança]]
- [[Generalização]]
- [[Pensamento de Caixa Preta]]
