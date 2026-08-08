Regra de design (*Don't Repeat Yourself*): evite duplicar a mesma lógica ou conhecimento em múltiplos pontos do sistema — mantenha uma única representação autoritativa.

## Na Prática (OO)
- **Métodos:** Extraem comportamento repetido.
- **[[Herança]] / [[Generalização]]:** Extraem atributos e comportamentos compartilhados entre classes.

## Por quê
- Sistemas com código repetido são mais difíceis de expandir, alterar e manter; uma correção exige editar vários lugares e é propensa a erro.

## Quando
- **Usar:** para manter uma única representação autoritativa de cada conhecimento/lógica.
- **Evitar:** abstrações forçadas que acoplam coisas só parecidas, não iguais.

## Conexões
- [[Generalização]]
- [[Herança]]
- [[Design Orientado a Objetos]]
