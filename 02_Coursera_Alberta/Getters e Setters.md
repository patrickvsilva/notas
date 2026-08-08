Métodos públicos que formam o “portão” de acesso a atributos privados — leem (getter) ou alteram (setter) o estado de forma controlada, preservando a integridade dos dados ([[Encapsulamento]] / [[Ocultação de Informação]]).

## Convenção de Nome
- **Getter:** `get` + NomeDoAtributo → retorna o valor (ex: `getGpa()`).
- **Setter:** `set` + NomeDoAtributo → altera o valor com segurança (ex: `setGpa(gpa)`).

## Mais do que ler/escrever
- Podem validar, rejeitar ou transformar valores (ex: `setDegreeProgram` só aceita se GPA > 2.7; `setGpa` rejeita nota fora da escala 0–4).
- O mundo externo não precisa saber dessas regras — só que o método cumpre o contrato ([[Pensamento de Caixa Preta]]).

## Conexões
- [[Ocultação de Informação]]
- [[Encapsulamento]]
- [[Modificadores de Acesso]]
- [[Visibilidade UML]]
- [[Diagrama de Classes]]
- [[Pensamento de Caixa Preta]]
