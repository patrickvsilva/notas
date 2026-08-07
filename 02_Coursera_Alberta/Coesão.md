Métrica de [[Complexidade de Design]] que captura a **clareza das responsabilidades** dentro de um módulo. Meta: coesão **alta** — um propósito claro (faz uma coisa bem); não baixa (vários propósitos misturados ou propósito indefinido).

## Sinais
- **Alta:** módulo com responsabilidade única e óbvia.
- **Baixa:** módulo tenta encapsular mais de um propósito → candidata a **dividir** ([[Decomposição]]).

## Exemplo
- `Sensor` que mede umidade **e** temperatura → **baixa** coesão.
- `HumiditySensor` + `TemperatureSensor`, cada um com um `get` claro → **alta** coesão (e melhora [[Acoplamento]] para quem usa).

## Conexões
- [[Complexidade de Design]]
- [[Acoplamento]]
- [[Decomposição]]
- [[Abstração]]
- [[Princípio da Menor Surpresa]]
- [[Cartões CRC]]
- [[Design Orientado a Objetos]]
