Mentalidade de tratar uma classe como uma caixa opaca: o consumidor fornece entradas e obtém saídas via métodos, sem precisar conhecer a representação interna dos atributos nem como os métodos calculam o resultado — alinhada a [[Ocultação de Informação]].

## Implicação
- O *como* fica interno; o *o quê* (contrato da interface) é o que importa para o mundo externo.
- Ex: pedir o GPA a um Estudante — não importa se veio de papel, banco de dados ou sistema online; o resultado é o mesmo.
- Ex: `String.concat` — você usa a assinatura; a implementação pode mudar.
- Ex. CS50: input → caixa → output ([[Resolução de Problemas]]); bloco Scratch `say` — você não implementa o balão.

## Quando
- **Usar:** ao consumir um módulo só pelo contrato (entradas/saídas), sem abrir a implementação.
- **Evitar:** depender de detalhes internos — quebra o encapsulamento e acopla.

## Conexões
- [[Ocultação de Informação]]
- [[Encapsulamento]]
- [[Barreira de Abstração]]
- [[Abstração]]
- [[Resolução de Problemas]]
- [[CS50]]
