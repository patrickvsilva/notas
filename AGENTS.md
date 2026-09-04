# AGENTS.md

Vault Obsidian pessoal de estudo em engenharia de software. Não é um repositório de código de produto.

Idioma das notas e das respostas sobre o vault: **português (pt-BR)**.

## Objetivo do aluno

Sintetizar com precisão, não acumular aula. Notas atômicas, enxutas, acionáveis, ligadas por `[[wikilinks]]`.

O desafio recorrente é a **paralisia pela importância**: escrever demais por medo de esquecer. O agente combate isso — enxuga, não expande.

## Mapa do vault

| Pasta / arquivo | Papel |
|---|---|
| `00_MBA/` | Visão **macro**: gestão, processo, qualidade. Hub: `MBA Engenharia de Software.md` |
| `01_CS50/` | Fundamentos de CS (Harvard). Hub: `CS50.md`. Prioridade: **depois** do Alberta |
| `02_Coursera_Alberta/` | Visão **micro**: OOD, UML, padrões, arquitetura, SOA. **Foco atual** |
| `03_RWTHx/` | Otimização matemática (RWTH/edX). Hub: `Otimização Matemática para Engenheiros.md`. Paralelo; não substitui Alberta |
| `Pendências Engenharia de Software.md` | Mapa de gaps e ordem das trilhas |
| `Templates/Conceito Design.md` | Template obrigatório para nota nova de conceito |
| `.agents/skills/revisor-software-design/` | Skill de tutor/revisor — usar ao revisar, validar, sintetizar ou formatar notas |

Hubs de trilha (não duplicar conteúdo neles; só mapa + pontes):

- `[[Pendências Engenharia de Software]]`
- `[[MBA Engenharia de Software]]`
- `[[CS50]]`
- `[[Especialização em Design e Arquitetura de Software]]`
- `[[Otimização Matemática para Engenheiros]]`

## Tipos de nota

**Hub** — índice da trilha ou disciplina: 1 parágrafo de propósito, tabela/lista de filhos, `## Conexões`.

**Atômica (conceito)** — um conceito por arquivo. Nome do arquivo = nome do conceito (ex.: `Encapsulamento.md` → `[[Encapsulamento]]`). Sem frontmatter YAML nas notas.

**Estudo de caso** — prefixo `Estudo de Caso - …` (ex.: `Estudo de Caso - Caixa Eletrônico.md`).

## Padrão ao criar ou editar nota de conceito

Partir de `Templates/Conceito Design.md`:

1. Primeira linha: definição em 1–2 frases (o que é e por que importa).
2. Corpo: bullets ou tabela curta. No máximo **um** exemplo canônico.
3. `## Quando` — **opcional.** Só se o conceito for decisão de design: **Usar:** 1 linha; **Evitar:** 1 linha. Hubs, vocabulário e definições factuais podem omitir.
4. `## Conexões` — 3 a 8 `[[links]]` fortes. Hubs podem ter mais; notas atômicas não.

Regras:

- Preferir `[[link]]` a repetir conteúdo de outra nota.
- Código **somente Java**, e só se esclarecer o conceito. Sem Python nem outras linguagens.
- Diagramas: Mermaid (`classDiagram`, `sequenceDiagram`, `flowchart`) ou UML ASCII curto.
- **Não** reescrever a nota do zero. Editar o mínimo para aderir ao padrão.
- Wikilink usa o nome do arquivo sem `.md`. Alias só quando o texto fluir melhor: `[[Eficiência de Algoritmos|eficiência]]`.

## Quando o usuário pede revisão

Ler e seguir `.agents/skills/revisor-software-design/SKILL.md`. Resposta em 4 blocos:

1. Precisão técnica (o que estava certo, depois o erro)
2. Enxugamento e formato
3. Prática (trade-off só se a nota já tiver `## Quando` ou se o conceito for claramente uma decisão de design)
4. 2–4 sugestões de `[[links]]`

Tom: mentor direto, crítico e encorajador. Destacar o que já está bem sintetizado antes das correções.

## Alberta (Univ. of Alberta / Coursera) — estado

Especialização em 4 cursos. O vault está sobretudo no **Course 1 (OOD)**. Ainda não existem as notas-hub `Padrões de Projeto.md` nem `Arquitetura Orientada a Serviços.md` (já linkadas em hubs).

1. OOD — princípios, CRC, UML, acoplamento/coesão
2. Design Patterns — GoF + code smells
3. Software Architecture — 4+1, estilos, atributos de qualidade / ATAM
4. SOA & Microservices — WS*, REST, microserviços

Pré-requisito do curso: Java. Exemplos nas notas acompanham isso.

## O que não fazer

- Não criar README, pastas novas ou sistema de tags sem pedido explícito.
- Não alterar `.obsidian/plugins/`, `workspace.json` ou `workspace-mobile.json` (estado da UI).
- Não versionar segredos; não commitar a menos que o usuário peça.
- Não gerar textos longos “completos” no lugar de uma síntese.
- Não misturar trilhas: MBA = gestão/processo; Alberta = design/arquitetura; CS50 = fundamentos; RWTHx = otimização matemática. Conectar com `[[links]]`, não fundir numa nota só.

## Git

Repo `patrickvsilva/notas`, branch `main`. Plugin Obsidian Git instalado. Commits só sob pedido explícito.
