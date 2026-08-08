Modelo comum de cor: misturar intensidades de **R**ed, **G**reen e **B**lue (0–255 cada = 1 [[Bit e Byte|byte]]). Um **pixel** é um ponto da imagem com uma cor RGB (~3 bytes).

## Ideia Central
- Mesmos bytes que em [[ASCII]] seriam `HI!` (`72,73,33`), em um editor de imagem são uma cor.
- `0,0,0` = preto; `255,255,255` = branco.
- Imagem = grade de pixels; vídeo ≈ muitas imagens/segundo; som ≈ números (frequência, duração, amplitude).

## Quando
- **Usar:** raciocinar tamanho de arquivos (muitos pixels × 3 bytes → MB) e filtros/edição.
- **Evitar:** tratar GIF/JPEG/PNG como “mágica” — no fundo são bits interpretados como cores.

## Conexões
- [[Bit e Byte]]
- [[ASCII]]
- [[Abstração]]
- [[CS50]]
