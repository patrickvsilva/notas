Princípio de design (Rule of Least Astonishment) que estabelece que um componente, abstração ou interface deve se comportar de forma intuitiva, capturando apenas características essenciais sem introduzir elementos surpreendentes ou fora do seu escopo.

## Aplicação em Design Orientado a Objetos

- **Escopo Delimitado:** Ao criar uma classe via [[Abstração]], o desenvolvedor deve incluir apenas os atributos e comportamentos diretamente relacionados ao contexto e propósito daquela entidade.
- **Eliminação de Irrelevâncias:** Detalhes secundários não devem ser inseridos "por garantia" (ex: adicionar o pet ou jogo favorito de um aluno dentro de uma abstração em ambiente acadêmico).
- **Previsibilidade:** Garante que outros desenvolvedores, ao consumir a classe ou modelo, encontrem exatamente o que esperam, sem comportamentos inesperados ou propriedades estranhas ao conceito.

## Benefícios
- Aumenta a legibilidade e manutenibilidade do código.
- Reduz a curva de aprendizado para novos desenvolvedores ao interagir com a API ou domínio.
- Evita a poluição de classes com responsabilidades desconexas.

## Quando
- **Usar:** para que abstrações e APIs se comportem exatamente como o nome/contexto sugerem.
- **Evitar:** atributos ou métodos “por garantia” fora do escopo — surpreendem quem consome.

## Conexões
- [[Abstração]]
- [[Design Orientado a Objetos]]
