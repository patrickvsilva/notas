Sistema de numeração **base 2**: só dígitos `0` e `1`. Cada coluna vale potência de 2 (1, 2, 4, 8, 16…), análogo ao decimal (base 10) com colunas 1, 10, 100….

## Ideia Central
- Decimal `123` = \(1×100 + 2×10 + 3×1\).
- Binário `111` = \(1×4 + 1×2 + 1×1 = 7\).
- Sem espaço para o próximo bit (overflow): contagem “volta” e gera bugs no mundo real.
- Dedos/luzes: posição importa — não só “quantos estão ligados”.

## Exemplo
```
binário 01000001 → colunas …64 32 16 8 4 2 1
                   → 64+1 = 65 → letra 'A' em [[ASCII]]
```

## Quando
- **Usar:** entender o que o hardware realmente armazena.
- **Evitar:** converter tudo mentalmente no dia a dia — o computador faz isso; você precisa do modelo mental.

## Conexões
- [[Bit e Byte]]
- [[ASCII]]
- [[Algoritmo]]
- [[CS50]]
