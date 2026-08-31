Dois programadores lado a lado no **mesmo computador**, no mesmo design/algoritmo/código/teste: um **condutor** (teclado) e um **navegador** (ativo: defeitos, alternativas, estratégia). Os dois **possuem** o artefato; os papéis revezam. Review e design no ato — não é “duas pessoas no trabalho de uma”. Prática anterior ao [[XP]]; o XP só a arranjou (e insiste em par no código de produção). Arranjo de **contexto definido** — Fabri não conhece quem emparelha o expediente inteiro.

## Ideia Central
- Embutido: review contínuo (quatro olhos — você não vê o próprio erro) e menos *design tunnel vision* (mais alternativas; modelagem em geral **mais simples**).
- Produtividade: a objeção é “desperdício de uma pessoa”. Williams (Utah): depois de **jellar**, ~15% mais horas-programador, calendário ~40–50% mais rápido, mais casos de teste; na 1ª tarefa o extra chega a ~60% (ajuste). Fabri: par só vale na complexidade **alta/muito alta**; baixa/média o ganho some — e inexperiente detecta o mesmo erro lógico que o individual.
- **Pressão do par:** compromisso compartilhado (e-mail/IM somem; o par puxa no cansaço e **não deixa largar a prática** quando aperta). Entrega mais consistente.
- **Revezamento:** condutor ↔ navegador **e** troca de pares — *um* par, não *o* par (qualquer um substitui). Com regra.
- **Conhecimento:** time nivelado **por alto** — código **e** regras de negócio. Júnior também puxa o sênior no detalhe (Jeffries/C3). Documento é frio.
- Caso: [[Estudo de Caso - Programação em Pares]] — calendário igual, qualidade no solver (solo retrabalhou).

## Onde no ciclo
- **Crítico:** análise e design juntos. Preparar **sozinho** antes (ler o problema, pensar a lógica, prototipar).
- **Implementação:** review no ato; simples/GUI o par costuma separar.
- **Teste:** menos crítico se os casos nasceram em par; podem rodar em duas máquinas e reencontrar no defeito.
- Trabalho solo: a maioria **revisa e incorpora**; XP puro raspa e refaz em par. Profissionais no paper da Williams também separam o rote — alinhado ao Fabri (não emparelhar baixa/média).

## Desafios
- Mesa que não cabe dois; gerência que conta “um salário = um código” (confunde hora-programador com calendário).
- Medo de mostrar código; ego **alto** (*my way*) ou **baixo** (não contribui); bônus por desempenho **individual** (competição mata ajuda — incompatível com [[XP]]).
- Humildade e paciência: o colega está aprendendo (vale também quem não conhece o **modelo de negócio**).

## Quando
- **Usar:** análise/design e implementação de complexidade alta/muito alta — e processo que a detecta cedo. Onboarding/nivelar saber é objetivo **outro**.
- **Evitar:** baixa/média ou GUI/rote como arranjo padrão; cobrar o 15% na primeira sessão (ainda não jellou); emparelhar o expediente inteiro; ranking individual; par sem espaço nem regra de troca; achar que par isolado = [[XP]].

## Conexões
- [[XP]]
- [[Métodos Ágeis]]
- [[Métodos Ágeis de Desenvolvimento de Software]]
- [[Integridade Conceitual]]
- [[Design de Software]]
- [[Manifesto Ágil]]
- [[Estudo de Caso - Programação em Pares]]
