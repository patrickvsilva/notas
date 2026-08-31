Extensão do [[Particionamento em Classes de Equivalência]]: os defeitos se concentram na **fronteira** — testar imediatamente abaixo, no limite e imediatamente acima.

## Ideia Central
- Intervalo [0, 10]: `-1`, `0`, `1`, `9`, `10`, `11`.
- Também a fronteira do **tipo**. `short` (16 bits): `-32769`, `-32768`, `-32767`, `32766`, `32767`, `32768` — primeiro e último fora do tipo; o programa deve recusar, não estourar.
- Caso: idade 0 / negativa / letra — [[Estudo de Caso - Teste de Cadastro]].

## Quando
- **Usar:** intervalo numérico, capacidade, tamanho de campo, overflow.
- **Evitar:** só o meio da classe válida.

## Conexões
- [[Particionamento em Classes de Equivalência]]
- [[Teste de Caixa Preta]]
- [[Estudo de Caso - Teste de Cadastro]]
- [[Requisitos Funcionais]]
