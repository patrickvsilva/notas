Mecanismo pelo qual uma **subclasse** recebe atributos e comportamentos de uma **superclasse**, permitindo reutilizar o que é comum e especializar o que é específico. É a forma principal de aplicar [[Generalização]] entre classes ([[Herança de Implementação]]).

## Ideia Central
- Relação *"é um"* (ex: Cachorro *é um* Animal).
- Superclasse = generalizada; subclasse = especializada (pode acrescentar e [[Sobrescrita de Método|sobrescrever]]).
- No diagrama e no código: **não** redeclara o que já veio da superclasse — a seta / `extends` já comunica isso.

## UML
Seta sólida com ponta triangular aberta: **cabeça = superclasse**, **cauda = subclasse**. Por convenção, aponta **para cima** (como árvore genealógica).

```
        Animal
       △
       │
      Dog
```

## Na Prática (código)
| Conceito | Java | Python |
|---|---|---|
| Herdar | `class Dog extends Animal` | `class Dog(Animal):` |
| Chamar super | `super(...)` | `super().__init__(...)` |
| Não instanciar a geral | `abstract class` ([[Classe Abstrata]]) | `ABC` / `@abstractmethod` |
| Atributo para subclasses | `protected` → `#` no UML ([[Visibilidade UML]]) | `_nome` (convenção) |

- Se a superclasse tem **construtor explícito**, a subclasse deve chamá-lo (`super`) para inicializar os atributos herdados.
- Em Java: **herança simples** — uma subclasse, uma só superclasse; uma superclasse pode ter muitas subclasses. A cadeia pode descer vários níveis.

### Exemplo (`Animal` → `Dog`)
```
        Animal
        ------
        # legs : int
        + walk()
           △
           │
          Dog
          ---
          + playFetch()
          + walk()   «override»
```

```java
public abstract class Animal {
    protected int legs;

    public Animal(int legs) {
        this.legs = legs;
    }

    public void walk() {
        System.out.println("walking");
    }
}

public class Dog extends Animal {
    public Dog() {
        super(4);
    }

    @Override
    public void walk() {
        System.out.println("I'd rather lay on the couch");
    }

    public void playFetch() { /* ... */ }
}
```

```python
from abc import ABC

class Animal(ABC):
    def __init__(self, legs: int):
        self._legs = legs

    def walk(self) -> None:
        print("walking")

class Dog(Animal):
    def __init__(self):
        super().__init__(4)

    def walk(self) -> None:
        print("I'd rather lay on the couch")

    def play_fetch(self) -> None:
        ...
```

> Em Python, `ABC` sozinho não impede instanciação; use `@abstractmethod` quando quiser o mesmo efeito do `abstract` do Java.
## Conexões
- [[Generalização]]
- [[Herança de Implementação]]
- [[Classe Abstrata]]
- [[Sobrescrita de Método]]
- [[Visibilidade UML]]
- [[Diagrama de Classes]]
- [[DRY]]
- [[Abstração]]
- [[Design Orientado a Objetos]]
