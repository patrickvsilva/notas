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
| Conceito | Java |
|---|---|
| Herdar | `class Dog extends Animal` |
| Chamar super | `super(...)` |
| Não instanciar a geral | `abstract class` ([[Classe Abstrata]]) |
| Atributo para subclasses | `protected` → `#` no UML ([[Visibilidade UML]]) |

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

## Quando
- **Usar:** relação *é-um* verdadeira + reuso de implementação compartilhada.
- **NÃO usar:** só para reutilizar código sem *é-um* — prefira colaboração ou [[Interface]].

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
