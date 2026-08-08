Princípio de design que reduz redundância ao extrair características ou comportamentos repetidos e reutilizá-los em um único lugar, em vez de duplicá-los pelo sistema.

## Duas Formas
- **Métodos:** Generalizam um comportamento repetitivo. O mesmo algoritmo/ação se aplica a conjuntos diferentes de dados via argumentos.
- **Classes ([[Herança]]):** Características comuns (atributos e comportamentos) entre duas ou mais classes são fatoradas em uma **superclasse**; as **subclasses** herdam o comum e podem acrescentar o que as especializa.

## Terminologia
- **Superclasse (pai):** Contém o que é compartilhado.
- **Subclasse (filho):** Herda o compartilhado e adiciona atributos/comportamentos específicos (ex: Gato e Cachorro herdam de Animal).

## Benefícios
- **[[DRY]] (Don't Repeat Yourself):** Menos código duplicado → menos erros ao alterar o comum.
- **Extensibilidade:** Novas subclasses ganham o comportamento comum sem reescrevê-lo.
- **Manutenibilidade:** Mudança no compartilhado ocorre em um só lugar (a superclasse ou o método).

## Na Prática
- No [[Diagrama de Classes]]: seta de [[Herança]] (superclasse no topo); não repetir atributos/métodos herdados na subclasse.
- No código: `extends` / herança de classe, [[Classe Abstrata]] quando o geral não deve ser instanciado, `super` no construtor, [[Sobrescrita de Método]] para especializar comportamento.
- Tipos: [[Herança de Implementação]] (simples em Java). Para contratos de comportamento sem herdar implementação: [[Interface]] ([[Subtipagem]], [[Polimorfismo]]) — *não* é generalizar classes.

## Quando
- **Usar:** características/comportamentos comuns a extrair num só lugar ([[DRY]]), com especialização real nas subclasses.
- **Evitar:** forçar [[Herança]] só para reutilizar código, ou violar [[Princípio de Substituição de Liskov]] — considere [[Decomposição]].

## Conexões
- [[Design Orientado a Objetos]]
- [[Herança]]
- [[Princípio de Substituição de Liskov]]
- [[Herança de Implementação]]
- [[Interface]]
- [[Decomposição]]
- [[DRY]]
- [[Classe Abstrata]]
- [[Sobrescrita de Método]]
