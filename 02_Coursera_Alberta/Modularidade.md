Qualidade de design em que o sistema é feito de partes com fronteiras claras: cada módulo faz o seu trabalho, pode ser reutilizado/substituído e alterado com pouco impacto nos demais.

## Como obter
- Principal alavanca: [[Separação de Preocupações]] (via os quatro princípios OO).
- Sinal de sucesso: alta [[Coesão]] dentro do módulo + conexões via contratos estreitos ([[Interface]], baixo [[Acoplamento]] indevido).

## Por quê importa
- Manutenção: bug/feature fica localizado.
- Reuso: dá para usar só a câmera, sem carregar o telefone (ex. da aula). Em escala de produto: [[Framework]] (você encaixa; o Frame chama).
- Flexibilidade: trocar uma implementação sem reescrever o coordenador.

## Quando
- **Usar:** quando partes com fronteiras claras precisam ser reutilizadas, trocadas ou alteradas com pouco impacto.
- **Evitar:** “módulos” sem contrato/fronteira — ou fatiar sem necessidade real.

## Conexões
- [[Separação de Preocupações]]
- [[Coesão]]
- [[Acoplamento]]
- [[Complexidade de Design]]
- [[Design Orientado a Objetos]]
- [[Decomposição]]
- [[Interface]]
- [[Framework]]
