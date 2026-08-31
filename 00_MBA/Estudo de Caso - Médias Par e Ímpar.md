Lê 5 inteiros, soma/conta pares e ímpares e imprime as duas médias. Happy path misto (`1 2 3 4 5`) passa. Classe vazia (5 ímpares ou 5 pares) → divisão por zero. Crash = disponibilidade: entrada trivial derruba o processo.

## Ideia Central
- Defeito: `soma / contagem` quando a contagem daquela classe é 0. O post deixa em aberto; o oráculo é o crash (e média errada se passar).
- [[Particionamento em Classes de Equivalência|Equivalência]]: todos pares | todos ímpares | misto | não-numérico. `0` é par. O cadastro testava *campo*; aqui a classe **vazia no agregado** ainda é classe.
- Secundário: média inteira trunca; overflow na soma. A provocação do Ismael (segurança) é o crash.
- Mesmo recado do [[Estudo de Caso - Teste de Cadastro]]: o que “sempre passa” não exercita o ramo que quebra.

## Exemplo

```java
System.out.println(somaPar / nPar);     // ArithmeticException se nPar == 0
System.out.println(somaImpar / nImpar);
```

## Quando
- **Usar:** todo agregado com denominador (média, taxa, “por tipo”) — incluir 0 elementos.
- **Evitar:** só a mistura 1–5; tratar crash como “não vai acontecer”.

## Conexões
- [[Teste de Caixa Preta]]
- [[Particionamento em Classes de Equivalência]]
- [[Estudo de Caso - Teste de Cadastro]]
- [[Atributos de Qualidade]]
- [[Requisitos Não-Funcionais]]
- [[Métodos Ágeis de Desenvolvimento de Software]]
