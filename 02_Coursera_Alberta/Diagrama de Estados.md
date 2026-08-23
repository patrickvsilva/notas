Diagrama [[UML]] que mostra **como um objeto (ou o sistema) se comporta** ao longo da vida: estados e eventos que os mudam.

## Ideia Central
- Complementa o [[Diagrama de Classes]] (estrutura) e o [[Diagrama de Sequência]] (conversa entre objetos): aqui o foco é **um** objeto reagindo a eventos.
- **Estado:** como o objeto existe num instante — determinado pelos valores dos atributos (carro automático: park, reverse, neutral, drive). Em cada estado, só certos comportamentos são possíveis.
- Útil para achar evento esquecido (ex: cancelar) e para guiar testes por estado.

## Notação
| Elemento | Desenho | Significado |
|---|---|---|
| Início | círculo cheio | estado inicial |
| Estado | retângulo arredondado | nome; opcional: variáveis e atividades |
| Transição | seta | evento `[guarda]` `/` ação |
| Término | círculo com ponto | objeto destruído / processo concluído (opcional) |

### Dentro do estado
- **Nome** — obrigatório e significativo (`Idle`, `Reverse`).
- **Variáveis** — dados relevantes naquele estado (ex: `total` de moedas; turma `full` quando matrículas = capacidade).
- **Atividades:** `entry` (ao entrar), `do` (enquanto permanece), `exit` (ao sair). Relógio no estado ringing: `entry` solta a mola; `do` toca o sino; `exit` relock a mola.

### Rótulo da transição
Sempre tem **evento**. Pode ter **guarda** (só transita se verdadeira) e **ação** (efeito da transição). Auto-transição = seta que volta ao mesmo estado.

## Exemplo (máquina de vendas)
Idle: variável `total`; `entry / display total`. EnoughCoins: `entry / display enough coins`. Sem término — o processo não acaba.

```mermaid
stateDiagram-v2
    [*] --> Idle
    Idle --> Idle: insert coin [total < price]\n/ display insert more coins
    Idle --> EnoughCoins: insert coin [total = price]
    EnoughCoins --> Idle: press dispense\n/ total = 0, dispense product
    Idle --> Idle: press cancel\n/ total = 0, eject coins
    EnoughCoins --> Idle: press cancel\n/ total = 0, eject coins
```

Término (não usado aqui): ATM devolve o cartão e o processo acaba — ver [[Estudo de Caso - Caixa Eletrônico]].

## Quando
- **Usar:** objeto com ciclo de vida claro; descobrir eventos/condições faltando; montar testes por estado.
- **Evitar:** objeto sem estados relevantes; no lugar de [[Diagrama de Sequência]] (não mostra colaboração) ou [[Diagrama de Classes]] (não mostra estrutura). Processos contínuos podem omitir término.

## Conexões
- [[UML]]
- [[Diagrama de Sequência]]
- [[Diagrama de Classes]]
- [[Encapsulamento]]
- [[Design Técnico]]
- [[Design Orientado a Objetos]]
- [[Estudo de Caso - Caixa Eletrônico]]
