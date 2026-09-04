Requisito em linguagem natural na voz do usuário: *como [papel], eu quero [objetivo] para que [motivo]*. Alimenta o OOD: substantivos → entidades; verbos → responsabilidades.

## Estrutura Padrão

> *"Como um **[papel do usuário]**, eu quero **[objetivo]** para que **[motivo]**."*

- **Papel do Usuário:** Quem utilizará a funcionalidade (ex: *Comprador Online*).
- **Objetivo:** O que o usuário pretende realizar.
- **Motivo:** A justificativa ou benefício (pode ser omitido se for óbvio).

## Mapeamento para [[Design Orientado a Objetos]] (OOD)
A análise sintática de uma User Story permite extrair os elementos fundamentais do sistema:

| Elemento Gramatical | Elemento de Software / OOD | Exemplo |
| :--- | :--- | :--- |
| **Substantivos** | [[Objetos de Entidade]] / Classes | *Comprador Online*, *Item*, *Carrinho de Compras* |
| **Verbos** | Responsabilidades / Métodos | *Adicionar*, *Comprar* (atribuídos ao Carrinho) |
| **Estrutura da Frase** | Conexões / Relacionamentos | *Comprador* possui conexão com *Carrinho*; *Carrinho* armazena múltiplos *Itens* |

## Conexões
- [[Levantamento de Requisitos]]
- [[Categorias de Objetos]]
- [[Design Conceitual]]
- [[Design Orientado a Objetos]]
- [[Métodos Ágeis de Desenvolvimento de Software]]
