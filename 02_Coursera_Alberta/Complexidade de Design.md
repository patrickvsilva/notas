Métricas e diretrizes para avaliar se a estrutura do software permanece **flexível, reutilizável e manutenível** — além de modelar com os quatro princípios OO e o [[Diagrama de Classes]].

## Por quê
- A memória de curto prazo humana segura ~**7** itens (Miller). Se a complexidade do design ultrapassa o que o desenvolvedor consegue “segurar na cabeça”, bugs aumentam.
- **Módulo** = qualquer unidade de programa (classe, método, etc.).

## Duas Lentes
| Métrica | Foco | Meta |
|---|---|---|
| [[Acoplamento]] | Complexidade **entre** o módulo e outros | **Baixo** / frouxo (Lego, não quebra-cabeça) |
| [[Coesão]] | Complexidade **dentro** do módulo | **Alta** (um propósito claro) |

## Quando
- **Usar:** [[Acoplamento]] baixo + [[Coesão]] alta para equilibrar flexibilidade e clareza.
- **Evitar:** otimizar só um lado — ↓ acoplamento pode ↓ coesão e vice-versa (a complexidade se redistribui).

## Conexões
- [[Separação de Preocupações]]
- [[Modularidade]]
- [[Acoplamento]]
- [[Coesão]]
- [[Design Orientado a Objetos]]
- [[Design de Software]]
- [[Decomposição]]
- [[Encapsulamento]]
- [[Abstração]]
- [[Generalização]]
