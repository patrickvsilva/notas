Mecanismo de linguagem para aplicar [[Ocultação de Informação]] / [[Encapsulamento]]: define **quem** pode ver ou chamar atributos e métodos.

## Quatro níveis (Java)
| Modificador | Quem acessa | UML |
|---|---|---|
| `public` | Qualquer classe | `+` |
| `protected` | A própria classe + **subclasses** + classes do **mesmo pacote** | `#` |
| *(default / package)* — sem palavra-chave | Só classes do **mesmo pacote** | `~` |
| `private` | Só a própria classe | `-` |

- Pacote (`package`) = namespace que agrupa classes relacionadas.
- Método `public`: outros **chamam** e recebem o resultado; **não** alteram a implementação (ela continua oculta).
- Atributo `public`: outros podem ler **e** modificar direto — use com parcimônia.

## Quando
- **Usar:** o nível mais restritivo que ainda permite o uso legítimo (ex: `-` + getters).
- **Evitar:** atributos `public` — qualquer um altera o estado sem controle.

## Conexões
- [[Ocultação de Informação]]
- [[Encapsulamento]]
- [[Visibilidade UML]]
- [[Herança]]
- [[Getters e Setters]]
- [[Diagrama de Classes]]
