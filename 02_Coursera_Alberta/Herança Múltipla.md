Quando uma subclasse tem **duas ou mais** superclasses. Útil em teoria, mas em Java **não é permitido** para classes — gera ambiguidade de dados/comportamento.

## Problema (ambiguidade)
Se duas superclasses declaram o mesmo atributo ou a mesma assinatura de método, a subclasse não saberia qual definição usar.

## Abordagem Java
- Classes: só [[Herança de Implementação]] **simples** (`extends` uma superclasse).
- Múltiplos tipos: a classe `implements` várias [[Interface|interfaces]].
- Assinaturas sobrepostas entre interfaces não são problema: a classe oferece **uma** implementação que satisfaz todos os contratos.

```java
public class Person implements ISpeaker, IGreeter {
    public void speak() { /* uma só definição */ }
}
```

> Em Python (e C++), herança múltipla de classes *é* possível — com trade-offs (ex: MRO). No curso, o modelo de referência é o do Java.

## Conexões
- [[Interface]]
- [[Herança de Implementação]]
- [[Herança]]
- [[Subtipagem]]
- [[Polimorfismo]]
