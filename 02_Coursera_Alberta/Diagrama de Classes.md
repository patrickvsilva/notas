Diagrama [[UML]] que representa uma [[Abstração]] como classe, com detalhe próximo o bastante do código para guiar a implementação — e conversível em ambas as direções (diagrama ↔ código).

## Estrutura da Caixa (3 seções)
```
+---------------------+
|   NomeDaClasse      |  → class (Java / Python)
+---------------------+
| propriedades        |  → atributos / variáveis de instância
+---------------------+
| operações           |  → métodos
+---------------------+
```
- **Propriedades:** nome + tipo (primitivo ou classe). Em Python o tipo é opcional (anotações).
- **Operações:** nome + parâmetros + tipo de retorno.
- **[[Visibilidade UML]]:** `+` público, `-` privado — aplica [[Encapsulamento]] no diagrama.

## Mapeamento ↔ Código
| Diagrama | Java | Python |
|---|---|---|
| Nome da classe | `class Nome` | `class Nome:` |
| Propriedade | variável de membro | atributo (`self.x` / `self._x`) |
| Operação | método | método (`def`, com `self`) |
| `+` / `-` | `public` / `private` | público / `_privado` (convenção) |

Conversão inversa: identificar classe → propriedades a partir dos atributos → operações a partir dos métodos (com params e retorno).

### Exemplo básico (`ClickCounter`)
```
+---------------------------+
| ClickCounter              |
+---------------------------+
| - count : int             |
+---------------------------+
| + setClickCount(c : int)  |
| + getClickCount() : int   |
+---------------------------+
```

```java
public class ClickCounter {
    private int count;

    public void setClickCount(int c) {
        count = c;
    }

    public int getClickCount() {
        return count;
    }
}
```

```python
class ClickCounter:
    def __init__(self):
        self._count = 0

    def set_click_count(self, c: int) -> None:
        self._count = c

    def get_click_count(self) -> int:
        return self._count
```

> Exemplo com validação em setter: ver [[Encapsulamento]] (`Student`).

## Relacionamentos (todo ↔ parte)
| UML | Relação | Notas |
|---|---|---|
| `———` linha | [[Associação]] | interação frouxa |
| `◇——` diamante vazio | [[Agregação]] | *has-a* fraco |
| `◆——` diamante cheio | [[Composição]] | *has-a* forte |
| `0..*`, `1`, … | [[Cardinalidade UML]] | quantos de cada lado |

Detalhes e código: ver [[Decomposição]].

## Relacionamento (generalização / tipos)
| UML | Relação | Notas |
|---|---|---|
| `──▷` seta sólida p/ cima | [[Herança]] | cabeça = superclasse; não repetir o herdado na subclasse |
| `╌╌▷` seta tracejada p/ cima | [[Interface]] (`implements`) | cabeça = `«interface»`; cauda = classe |
| `#` | [[Visibilidade UML]] | `protected` — visível às subclasses |

Detalhes e código: ver [[Generalização]] / [[Herança]] / [[Interface]].

## vs [[Cartões CRC]]
- CRC mistura “saber” e “fazer”; o diagrama **separa** propriedades e operações.
- CRC é ambíguo demais para traduzir direto em código; o diagrama remove essa ambiguidade.
- CRC permanece melhor para prototipar (barato, longe do código); o diagrama é melhor para comunicar o design técnico.

## Conexões
- [[UML]]
- [[Cartões CRC]]
- [[Abstração]]
- [[Encapsulamento]]
- [[Visibilidade UML]]
- [[Getters e Setters]]
- [[Decomposição]]
- [[Associação]]
- [[Agregação]]
- [[Composição]]
- [[Cardinalidade UML]]
- [[Generalização]]
- [[Herança]]
- [[Interface]]
- [[Subtipagem]]
- [[Polimorfismo]]
- [[Classe Abstrata]]
- [[Sobrescrita de Método]]
- [[Design Técnico]]
- [[Design Conceitual]]
- [[Design Orientado a Objetos]]
