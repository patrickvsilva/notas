Métrica de [[Complexidade de Design]] que captura quão difícil é **conectar** um módulo a outros. Meta: acoplamento **baixo / frouxo** (como Lego — peças compatíveis e substituíveis), não alto / apertado (como peças de quebra-cabeça que só encaixam em um lugar).

## Três Critérios
| Critério | Pergunta | Meta |
|---|---|---|
| **Grau** | Quantas conexões com outros módulos? | Poucas (parâmetros / interfaces estreitas) |
| **Facilidade** | A conexão é óbvia sem ler a implementação alheia? | Alta — respeita [[Encapsulamento]] / [[Pensamento de Caixa Preta]] |
| **Flexibilidade** | Os outros módulos são trocáveis depois? | Alta — substituíveis |

## Exemplo (anti-padrão → melhor)
- `Sensor.get(flag)` com `0` = umidade, `1` = temperatura → quem chama precisa “abrir” o método para entender o flag → **falta facilidade** → chamador fica **fortemente acoplado**.
- Separar `HumiditySensor.get()` e `TemperatureSensor.get()` → intenção clara → uso **frouxamente acoplado**.

## Conexões
- [[Separação de Preocupações]]
- [[Modularidade]]
- [[Complexidade de Design]]
- [[Coesão]]
- [[Encapsulamento]]
- [[Decomposição]]
- [[Interface]]
- [[Objetos de Controle]]
- [[Design Orientado a Objetos]]
