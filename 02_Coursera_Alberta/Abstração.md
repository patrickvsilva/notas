Processo de simplificar um conceito do domínio do problema focando apenas nos seus aspectos essenciais dentro de um contexto específico, descartando detalhes irrelevantes para a solução.

## Pilares da Abstração

- **Contexto e Perspectiva:** A abstração é sempre relativa ao propósito do sistema. O mesmo conceito real possui diferentes abstrações conforme o contexto:
  - Ex: Uma *Pessoa* no contexto de um aplicativo de trânsito é modelada como *Motorista*; em um aplicativo de restaurante, é modelada como *Cliente*.
  - Ex: Um *Estudante* no contexto **acadêmico** foca em *disciplinas*, *notas* e *matrícula*; no contexto **social**, foca em *grupos*, *hobbies* e *esportes*.
- **Estruturação em Classes:** Em [[Design Orientado a Objetos]], a abstração é formalizada em uma **Classe** (template), que define:
  - **Atributos:** Características/estado essenciais (a estrutura do atributo permanece, embora seu valor mude ao longo do tempo, como a nota de uma matéria).
  - **Comportamentos:** Ações e responsabilidades da abstração (ex: estudar, realizar tarefas).
  - *Ponte:* a abstração seleciona o essencial; o [[Encapsulamento]] agrupa e protege esses elementos na classe.
  - *Representação:* no design, a classe aparece no [[Diagrama de Classes]]; depois vira código.
- **[[Princípio da Menor Surpresa]] (Rule of Least Astonishment):** A abstração deve capturar apenas o que é estritamente esperado para o conceito, sem incluir atributos ou métodos fora do seu escopo de atuação.
- **Natureza Dinâmica:** Abstrações não são estáticas. Se as necessidades do negócio ou o problema mudarem, a abstração deve ser atualizada para refletir o novo contexto.

## Benefícios
- **Redução de Complexidade:** Permite focar no essencial de alto nível sem poluição visual ou lógica de detalhes secundários.
- **Classes Focadas e Sucintas:** Facilita a leitura, manutenção e compreensão do código por outros desenvolvedores.
- **Alinhamento com o Domínio:** Facilita a comunicação entre stakeholders e equipe técnica ao utilizar a linguagem do contexto.

## Conexões
- [[Design Orientado a Objetos]]
- [[Princípio da Menor Surpresa]]
- [[Encapsulamento]]
- [[Decomposição]]
- [[Generalização]]
- [[Diagrama de Classes]]
- [[Cartões CRC]]
