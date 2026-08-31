Técnica de [[Teste de Caixa Preta]]: agrupar o domínio em classes que o programa deve tratar igual — um representante por classe. Substitui o teste exaustivo, inviável (2³² × 2³² = 2⁶⁴ entradas; ver explosão em [[Model Checking]]).

## Ideia Central
- Inteiro em [0, 10]: três classes — abaixo, dentro, acima. Representantes: `-3`, `4`, `15`.
- Classe inválida extra: tipo errado (letra, nulo, branco) — não é outra técnica.
- Agregado (média de pares): **0 elementos** da classe ainda é classe — divide por zero. [[Estudo de Caso - Médias Par e Ímpar]].
- [[Análise do Valor Limite]] parte daqui e testa a fronteira.

## Quando
- **Usar:** domínio grande demais para enumerar.
- **Evitar:** um único happy path e chamar de testado — [[Estudo de Caso - Teste de Cadastro]].

## Conexões
- [[Teste de Caixa Preta]]
- [[Análise do Valor Limite]]
- [[Model Checking]]
- [[Estudo de Caso - Teste de Cadastro]]
- [[Estudo de Caso - Médias Par e Ímpar]]
- [[Requisitos Funcionais]]
- [[Caixa Preta]]
