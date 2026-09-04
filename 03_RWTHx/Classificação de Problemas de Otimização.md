Taxonomia do [[Problema de Otimização]] segundo o tipo da função, das restrições e das variáveis. A classe escolhe o algoritmo — formular primeiro, classificar depois.

## Ideia Central
Eixos usuais:

- **Linearidade.** Tudo linear → LP (programação linear). Alguma não-linearidade → NLP. NLP ainda pode ser convexo ou não, suave ou não.
- **Variáveis.** Só contínuas; só inteiras (IP); mistura (MIP / MILP / MINLP). Inteiro explode combinatória.
- **Tempo.** Estático: $x$ é um vetor. Dinâmico / controle ótimo (OCP): o DOF é uma *função do tempo* (trajetória, dosagem, movimento do robô).
- **Incerteza.** Determinístico: dados conhecidos. Estocástico: dados aleatórios (preço, vento); robusto: pior caso numa faixa.

Também: um vs vários objetivos; um nível vs bilevel (ótimo de um problema entra como restrição de outro).

**NLP vs OCP vs estocástico** (a pergunta da aula): NLP é estático e determinístico, possivelmente não linear. OCP acrescenta dinâmica no tempo. Estocástico acrescenta aleatoriedade no modelo. Podem combinar (OCP sob incerteza).

O divisor de águas na prática não é linear vs não linear, e sim [[Convexidade|convexo]] vs não convexo (Rockafellar).

## Quando
- **Usar:** depois de formular, antes de escolher solver.
- **Evitar:** pegar um algoritmo “genérico” e forçar o modelo a caber nele.

## Conexões
- [[Problema de Otimização]]
- [[Problema Convexo]]
- [[Convexidade]]
- [[Graus de Liberdade]]
- [[Otimização Matemática para Engenheiros]]
