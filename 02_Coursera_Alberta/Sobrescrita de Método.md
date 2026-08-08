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
- **Usar:** para especializar o *como* de um método herdado sem mudar a assinatura.
- **Evitar:** alterar o contrato ou surpreender quem usa o tipo da superclasse.

## Conexões
- [[Herança]]
- [[Generalização]]
- [[Pensamento de Caixa Preta]]
