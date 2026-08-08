Fronteira criada pelo [[Encapsulamento]] entre o que o mundo externo vê de uma classe (interface) e como ela funciona internamente.

## Efeito
- Reduz complexidade para quem usa a classe: detalhes internos deixam de ser relevantes.
- Aumenta reutilização: basta conhecer o método certo, seus argumentos e seus efeitos/saídas.

## Quando
- **Usar:** para isolar consumidores da complexidade interna e permitir mudança de implementação.
- **Evitar:** vazar detalhes através da barreira (consumidores acoplados ao *como*).

## Conexões
- [[Encapsulamento]]
- [[Pensamento de Caixa Preta]]
- [[Abstração]]
