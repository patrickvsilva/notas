Dois (ou mais) tipos compartilham a **mesma descrição** de um comportamento, mas cada um pode ter **implementação diferente**.

## Exemplo
- Contrato: `speak()` ([[Interface]] `IAnimal` ou método em [[Classe Abstrata]]).
- `Dog.speak()` → late; `Cat.speak()` → mia.
- Quem usa o tipo `IAnimal` pede `speak()` sem saber qual implementação roda ([[Pensamento de Caixa Preta]]).

## Como obter (Java)
- Via [[Interface]] (`implements`) ou via herança / [[Classe Abstrata]] com [[Sobrescrita de Método]].

## Quando
- **Usar:** quando vários tipos compartilham o mesmo contrato com implementações diferentes.
- **Evitar:** quando o comportamento deve ser único/fixo — polimorfismo só adiciona indireção.

## Conexões
- [[Interface]]
- [[Subtipagem]]
- [[Sobrescrita de Método]]
- [[Classe Abstrata]]
- [[Herança]]
- [[Design Orientado a Objetos]]
