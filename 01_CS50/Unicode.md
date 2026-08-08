Superset moderno do [[ASCII]] que representa (quase) todas as escritas humanas — e emojis — usando mais bits (até 32) por caractere (~bilhões de pontos de código).

## Ideia Central
- ASCII (~256) não cabe acentos, CJK, etc.
- Emoji = caracteres Unicode desenhados como imagens; o **mesmo código** pode parecer diferente no iOS vs Android (fonte gráfica).
- Mais bits → explosão de símbolos possíveis.

## Quando
- **Usar:** texto internacional e emojis no software moderno.
- **Evitar:** assumir “1 byte = 1 caractere” — em Unicode um caractere pode ocupar vários bytes.

## Conexões
- [[ASCII]]
- [[Bit e Byte]]
- [[CS50]]
