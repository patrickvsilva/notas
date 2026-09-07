Verificação sistemática do modelo de estados do software: a ferramenta explora **todos** os estados alcançáveis e diz se as propriedades valem — ou devolve um **contraexemplo**.

## Ideia Central
- Três jeitos de conferir se o sistema faz o que deve: **teste** (amostra caminhos), **prova** (tratar o programa como objeto matemático) e **model checking** (enumerar estados à máquina). Prova à mão falha nos casos especiais da concorrência; o checker existe para isso.
- Propriedade = afirmação sobre estado — às vezes no tempo (“se o ingresso A foi vendido, em todo estado futuro tem um só dono”). Ex.: o mesmo ingresso nunca é vendido a dois clientes; o sistema nunca entra em *deadlock* (espera circular: cada um segura o que o outro precisa, nada avança).
- Resultado: propriedade vale, **ou** contraexemplo (a sequência de eventos que quebrou a regra). Contraexemplo vira caso de teste.

### Explosão do espaço de estados
$n$ bits → $2^n$ estados. Na prática, da ordem de $2^{40}$. O modelo precisa ser **pequeno**: extrair do código só o que importa para a propriedade (*small world* — o defeito costuma aparecer no caso pequeno; ex.: 1–2 itens no pedido, não os totais). Extração automática ainda é o gargalo. Primo inviável no teste: enumerar todas as entradas — [[Particionamento em Classes de Equivalência]].

### Três fases
| Fase | O que fazer |
|---|---|
| Modelagem | Descrever o modelo + as propriedades. Antes: *sanity checks* (erros óbvios), para o checker focar no difícil. |
| Execução | Rodar o checker contra as propriedades. |
| Análise | Propriedade ok ou contraexemplo → corrigir → repetir. |

## Quando
- **Usar:** concorrência, protocolos, invariantes difíceis de acertar com teste (deadlock, *race*, “nunca dois donos do mesmo ingresso”) — depois do [[Diagrama de Estados]], não no lugar do teste.
- **Evitar:** modelo que não cabe em poucos bits; código em que o investimento não se justifica. Pouco do código escrito se beneficia.

## Conexões
- [[Diagrama de Estados]]
- [[Design Orientado a Objetos]]
- [[Design Técnico]]
- [[Requisitos Funcionais]]
- [[Atributos de Qualidade]]
- [[MBA Engenharia de Software]]
- [[Particionamento em Classes de Equivalência]]
- [[Teste de Caixa Preta]]
