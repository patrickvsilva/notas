Comparativo didático entre a arquitetura/design de uma residência e o design de software de um sistema de busca de cursos universitários.

## 1. Analogia da Casa
- **[[Levantamento de Requisitos]]:** Investigação inicial. Descobrir que o cliente quer 3 quartos, academia e banheiro, mas questionar a ausência da cozinha, tamanho dos cômodos, orientação solar e restrições locais de construção.
- **[[Design Conceitual]]:** Mapear cômodos (componentes), portas/corredores (conexões) e funções de cada cômodo (responsabilidades — ex: a academia fornece espaço/energia para equipamentos). *Sem detalhar tubulação ou fiação.*
- **[[Design Técnico]]:** Quebrar componentes (ex: o piso da academia precisará suportar pesos olímpicos, exigindo vigas no porão). Resolução de trade-offs (vigas no porão vs espaço amplo desejado no porão).

---

## 2. Aplicação em Software (Portal de Cursos)
- **Requisito do Usuário ([[História de Usuário]]):** *"Como aluno, quero buscar cursos relevantes através de uma página de busca."*
- **[[Design Conceitual]] (UI Mockup):**
  - **Componentes:** `Search Page`, `Course`.
  - **Identificação de lacunas:** Como o termo é digitado? Como os resultados são exibidos?
  - **Refinamento:** `Search Page` conecta-se a `Input Field`, `Search Button` e `Result Page`.
- **[[Design Técnico]] (Diagramas de Componentes/Classes):**
  - Conexão entre a `Search Page` e o `Course Database` pré-existente.
  - Decomposição das páginas e telas em coleções de classes, métodos e funções prontas para codificação.

## Conexões
- [[Fluxo de Desenvolvimento de Software]]
- [[Design Conceitual]]
- [[Design Técnico]]
