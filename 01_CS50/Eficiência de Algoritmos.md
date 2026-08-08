Quão rápido (ou com que recurso) um [[Algoritmo]] cresce quando o **tamanho do problema** *n* aumenta — correto ≠ bom o bastante.

## Ideia Central
Exemplo da lista telefônica (*n* páginas):

```mermaid
flowchart LR
    subgraph lento["~ n"]
        A[1 página por vez]
    end
    subgraph meio["~ n/2"]
        B[2 páginas + ajuste]
    end
    subgraph rápido["~ log₂ n"]
        C[meio → descarta metade]
    end
```

- Linear: dobrar *n* ≈ dobrar o tempo.
- Logarítmico (dividir ao meio): dobrar *n* ≈ **+1** passo.
- Meta de bom design: correto **e** eficiente (CPU, RAM, tempo, dinheiro).

## Quando
- **Usar:** comparar abordagens quando *n* pode ficar grande (dados, usuários).
- **Evitar:** otimizar cedo demais um *n* minúsculo — clareza primeiro.

## Conexões
- [[Algoritmo]]
- [[Resolução de Problemas]]
- [[CS50]]
