Verificação contra a especificação **sem** abrir o código: o testador escolhe entradas e observa saídas. ≠ [[Pensamento de Caixa Preta]] (design: consumir pelo contrato). Mapa: [[Caixa Preta]].

## Ideia Central
- Quatro tarefas: casos → dados → executar → verificar. Caso = o quê testar + técnica dos dados; HW/SW é plano, não o caso.
- Dados: [[Particionamento em Classes de Equivalência]] e [[Análise do Valor Limite]]. Letra, nulo, branco = classe inválida — Fabri às vezes chama de “teste funcional”; na literatura, funcional *é* esta família.
- Exaustivo (todas as entradas) é inviável — mesma explosão de [[Model Checking]], objeto diferente (inputs vs estados).
- Casos: [[Estudo de Caso - Teste de Cadastro]] (campo sem validar); [[Estudo de Caso - Médias Par e Ímpar]] (classe vazia no denominador). Caminho feliz não é teste.

## Quando
- **Usar:** validar o produto contra a spec, sem o fonte.
- **Evitar:** só os casos que “vão passar”; misturar com inspeção de código.

## Conexões
- [[Caixa Preta]]
- [[Pensamento de Caixa Preta]]
- [[Particionamento em Classes de Equivalência]]
- [[Análise do Valor Limite]]
- [[Requisitos Funcionais]]
- [[Estudo de Caso - Teste de Cadastro]]
- [[Estudo de Caso - Médias Par e Ímpar]]
- [[Model Checking]]
