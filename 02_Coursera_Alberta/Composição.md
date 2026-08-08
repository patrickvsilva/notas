Relação *has-a* **forte** da [[Decomposição]]: contenção exclusiva — o todo não existe sem suas partes; destruir o todo destrói as partes. Em geral, as partes só são acessadas via o todo.

## Sinais
- Partes exclusivas do todo (não compartilhadas).
- Lifetimes acoplados: criados e destruídos juntos.
- Acesso às partes costuma passar pelo todo.

## UML
Diamante **preenchido** (◆) no lado do **todo**.

```
House ◆── 1..* Room
Human ◆── 1 Brain
Employee ◆── 1 Salary
```

## Código (parte criada com o todo)
```java
public class Human {
    private Brain brain;

    public Human() {
        this.brain = new Brain();
    }
}
```

O `Brain` nasce no construtor do `Human`; não é passado de fora nem compartilhado.

## Quando
- **Usar:** *has-a* forte e exclusivo, com lifetimes acoplados.
- **Evitar:** se as partes precisam ser compartilhadas ou reutilizadas fora do todo — use [[Agregação]].

## Conexões
- [[Decomposição]]
- [[Associação]]
- [[Agregação]]
- [[Cardinalidade UML]]
- [[Diagrama de Classes]]
