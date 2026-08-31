Cadastro de pessoa (código, nome, rua, número, bairro, idade, CPF) + persistir. Nove profissionais juraram “está testado”; 7 casos de borda/inválido → 47 falhas em 63 (74%). Alunos de 6º semestre: 97%. Caminho feliz não é teste.

## Ideia Central
- Pedido: testem antes de entregar. Happy path típico: código `1`, Pedro Álvares Cabral, idade `25` — e o time encerra.
- Casos que o Fabri pediu depois: código 0 e negativo; nome branco; idade 0, negativa e letra; CPF inválido. São [[Particionamento em Classes de Equivalência|equivalência]] + [[Análise do Valor Limite|limite]] + tipo errado — [[Teste de Caixa Preta]].
- 9 × 7 = 63; 47 erros; 5,22 por pessoa. O programa “só” grava uma linha.
- Lição: teste é processo, não umas execuções que passam. Formalizar cedo (disciplina introdutória). Mesmo recado, outro defeito: [[Estudo de Caso - Médias Par e Ímpar]].

## Quando
- **Usar:** lembrar que “rodei e gravou” ≠ testado; treinar validação, não só o caminho feliz.
- **Evitar:** copiar 74%/97% como métrica do seu time.

## Conexões
- [[Teste de Caixa Preta]]
- [[Particionamento em Classes de Equivalência]]
- [[Análise do Valor Limite]]
- [[Requisitos Funcionais]]
- [[Estudo de Caso - Médias Par e Ímpar]]
- [[Métodos Ágeis de Desenvolvimento de Software]]
- [[MBA Engenharia de Software]]
