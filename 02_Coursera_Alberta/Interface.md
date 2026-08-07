Contrato de **comportamentos** (só assinaturas de métodos) que define um **tipo** sem fornecer implementação. Classes que o cumprem (`implements`) tornam-se subtipos desse contrato ([[Subtipagem]]).

> Não é classe e **não** é [[Generalização]] de um conjunto de classes: não traz atributos, construtores nem corpos de método — só o *o quê* fazer, não o *como*.

## Características
- Em Java: `interface IAnimal { void move(); void speak(); void eat(); }` (prefixo `I` por convenção).
- Em Python: paralelo próximo = `Protocol` / `ABC` só com `@abstractmethod`.
- Uma classe pode implementar **várias** interfaces (vários tipos ao mesmo tempo).
- Interfaces podem herdar de outras interfaces — só se o subcontrato puder **substituir** o supercontrato (ex: `IVehicleMovement3D` estende movimento 2D; não inchando o 2D com eixo Z).

## UML
Caixa com `«interface»` (guillemets). Seta **tracejada** com ponta triangular: cabeça = interface, cauda = classe; aponta **para cima**.

```
    «interface»
      IAnimal
         △
         ╎
        Dog
```

## Código
```java
public interface IAnimal {
    void move();
    void speak();
    void eat();
}

public class Dog implements IAnimal {
    public void move() { /* ... */ }
    public void speak() { System.out.println("bark"); }
    public void eat() { /* ... */ }
}
```

```python
from typing import Protocol

class Animal(Protocol):
    def move(self) -> None: ...
    def speak(self) -> None: ...
    def eat(self) -> None: ...

class Dog:
    def move(self) -> None: ...
    def speak(self) -> None:
        print("bark")
    def eat(self) -> None: ...
```

## Quando usar (vs [[Herança de Implementação]])
- Precisa de **contrato compartilhado** e implementações diferentes ([[Polimorfismo]]) sem herdar estado/código.
- Precisa de **múltiplos tipos** sem [[Herança Múltipla]] de classes (Java).
- Não use para “juntar métodos num balde grande” — só quando classes relacionadas devam trabalhar de forma consistente sob o mesmo tipo.

## Conexões
- [[Subtipagem]]
- [[Polimorfismo]]
- [[Herança de Implementação]]
- [[Herança Múltipla]]
- [[Classe Abstrata]]
- [[Diagrama de Classes]]
- [[Pensamento de Caixa Preta]]
