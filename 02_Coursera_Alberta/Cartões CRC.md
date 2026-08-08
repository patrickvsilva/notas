Técnica tátil e visual de modelagem de baixo custo usada no [[Design Conceitual]] para organizar componentes, identificar responsabilidades e simular a colaboração entre classes.

## O que é CRC?
**CRC** é um acrônimo para:
- **C**lass (Classe): Nome do componente/objeto candidato.
- **R**esponsibility (Responsabilidade): O que a classe deve saber ou fazer.
- **C**ollaborator (Colaborador): Outras classes com as quais ela se conecta para cumprir suas responsabilidades.

## Estrutura do Cartão CRC

```markdown
+----------------------------------------------------+
|                [ NOME DA CLASSE ]                  |
+--------------------------+-------------------------+
| Responsabilidades        | Colaboradores           |
| - O que a classe faz     | - Outras classes com as |
| - O que a classe sabe    |   quais ela interage    |
+--------------------------+-------------------------+
```

## Por que usar Cartões Físicos?
1. **Espaço Limitado por Design:** O tamanho reduzido força a decomposição de componentes grandes em classes menores e focadas.
2. **Experimentação & Simulação:** Permite que a equipe manipule os cartões, faça *role-playing* do fluxo e descubra componentes ocultos.
3. **Barato e Longe do Código:** Facilita descartar designs e mantém o foco no problema, não na implementação.

## Quando
- **Usar:** prototipagem conceitual barata — responsabilidades, colaboradores e role-playing.
- **Evitar:** como artefato único para implementação — avance para [[Diagrama de Classes]] e [[Diagrama de Sequência]].

## Conexões
- [[Design Conceitual]]
- [[Diagrama de Classes]]
- [[Diagrama de Sequência]]
- [[UML]]
- [[Estudo de Caso - Caixa Eletrônico]]
- [[Design Orientado a Objetos]]
- [[Design Técnico]]
