Contrato de **comportamentos** (só assinaturas de métodos) que define um **tipo** sem fornecer implementação. Classes que o cumprem (`implements`) tornam-se subtipos desse contrato ([[Subtipagem]]).

> Não é classe e **não** é [[Generalização]] de um conjunto de classes: não traz atributos, construtores nem corpos de método — só o *o quê* fazer, não o *como*.

## Características
- Em Java: `interface IAnimal { void move(); void speak(); void eat(); }` (prefixo `I` por convenção).
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

## Quando
- **Usar:** contrato compartilhado entre tipos distintos, ou múltiplos tipos sem herança múltipla.
- **Evitar:** se precisa de estado/implementação compartilhada — prefira [[Classe Abstrata]]/`extends`.

## Conexões
- [[Integridade Conceitual]]
- [[Subtipagem]]
- [[Polimorfismo]]
- [[Herança de Implementação]]
- [[Herança Múltipla]]
- [[Classe Abstrata]]
- [[Diagrama de Classes]]
- [[Pensamento de Caixa Preta]]
