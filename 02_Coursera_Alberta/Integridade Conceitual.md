Consistência do software: decisões de design e implementação alinhadas de modo que, mesmo com várias pessoas, o sistema pareça obra de **uma só mente**.

> Não silencia opinião — é acordo coletivo sobre princípios, convenções e estrutura.

Fred Brooks (*The Mythical Man-Month*): melhor omitir features anômalas e refletir **um** conjunto de ideias do que juntar muitas ideias boas, porém independentes e descoordenadas.

## Como alcançar
| Abordagem | Ideia |
|---|---|
| **Comunicação** | Acordos de time (stand-ups, retrospectivas, convenções de nome, libs/métodos padrão) |
| **Code review** | Exame sistemático linha a linha — acha bugs **e** alinha estilo/design |
| **Princípios e construtos** | [[Interface]], [[Padrões de Projeto]], princípios OO → comportamentos e estruturas previsíveis |
| **Design / [[Arquitetura de Software]]** | Blueprint compartilhado (processo único vs vários processos — ver [[Arquitetura vs Design de Software]]) |
| **[[Unificação de Conceitos]]** | Tratar coisas diferentes pelo mesmo modelo (ex: Unix — “tudo é arquivo”) |
| **Núcleo pequeno** | Poucas pessoas (ou uma) aceitam commits e guardam a visão geral |

## Por quê importa
- Time sabe *onde* e *como* mudar para novos requisitos.
- Menos “casos especiais” → manutenção e raciocínio mais baratos (metáfora: um canal de convites vs três redes sociais).

## Conexões
- [[Unificação de Conceitos]]
- [[Arquitetura vs Design de Software]]
- [[Arquitetura de Software]]
- [[Design de Software]]
- [[Design Orientado a Objetos]]
- [[Interface]]
- [[Separação de Preocupações]]
- [[Princípio da Menor Surpresa]]
- [[Padrões de Projeto]]
- [[Análise de Trade-offs]]
