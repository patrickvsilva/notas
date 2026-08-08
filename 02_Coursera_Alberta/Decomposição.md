Princípio de design que divide um todo em partes com responsabilidades distintas — ou, no sentido inverso, combina partes para formar um todo. Torna problemas complexos mais fáceis de entender e resolver.

## Ideia Central
- Separar pelas **responsabilidades** do todo: cada parte fica com um propósito específico.
- O todo pode **delegar** responsabilidades às partes (ex: geladeira delega congelar ao freezer).
- Partes podem ser, elas mesmas, um todo com subpartes (decomposição aninhada — ex: painel de instrumentos contém hodômetro, velocímetro).
- Funciona junto com os outros princípios: partes encapsuladas são tratadas como [[Pensamento de Caixa Preta|caixas pretas]].

## Questões Importantes (todo ↔ parte)
- **Cardinalidade fixa vs dinâmica:** número constante ao longo da vida do todo (ex: 1 motor) versus número que varia (ex: passageiros, prateleiras). No UML: [[Cardinalidade UML]].
- **Ciclo de vida:** lifetimes *acoplados* (parte não existe sem o todo — ex: freezer e geladeira) versus *independentes* (ex: comida e geladeira; pneus e carro).
- **Compartilhamento:** a mesma parte pode pertencer a vários todos ao mesmo tempo (ex: pessoa em duas famílias) — ou ser exclusiva (comida não está na geladeira e no forno ao mesmo tempo).

## Na Prática — Três Relacionamentos
Do mais frouxo ao mais rígido:

| Relação | Ideia | UML | Ciclo de vida |
|---|---|---|---|
| [[Associação]] | Interação frouxa; nenhum “tem” o outro de forma estrutural | linha reta | independentes |
| [[Agregação]] | *has-a* fraco; o todo tem partes, mas elas vivem sozinhas | ◇ diamante vazio no todo | independentes; compartilhamento ok |
| [[Composição]] | *has-a* forte; contenção exclusiva | ◆ diamante preenchido no todo | acoplados; destruir o todo destrói as partes |

## Benefícios
- **Complexidade gerenciável:** todo complicado = partes mais simples e separadas — base para alta [[Coesão]] e baixo [[Acoplamento]] ([[Complexidade de Design]]).
- **Responsabilidades claras:** facilita manutenção e raciocínio local.
- **Reutilização e paralelismo:** partes bem delimitadas podem ser reaproveitadas e desenvolvidas em paralelo.

## Quando
- **Usar:** para partir um todo complexo em partes com responsabilidades distintas.
- **Evitar:** decompor sem decidir ciclo de vida, cardinalidade e compartilhamento.

## Conexões
- [[Separação de Preocupações]]
- [[Modularidade]]
- [[Design Orientado a Objetos]]
- [[Associação]]
- [[Agregação]]
- [[Composição]]
- [[Cardinalidade UML]]
- [[Diagrama de Classes]]
- [[Complexidade de Design]]
- [[Acoplamento]]
- [[Coesão]]
- [[Encapsulamento]]
- [[Pensamento de Caixa Preta]]
- [[Abstração]]
- [[Generalização]]
- [[Categorias de Objetos]]
