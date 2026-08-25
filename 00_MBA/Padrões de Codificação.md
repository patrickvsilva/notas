Convenção compartilhada de estilo (indentação, chaves, nomes, comentários) para o time ler o mesmo código. Prática [[XP]]; **não** é [[Padrões de Projeto]].

## Ideia Central
- Estilo pessoal atrapalha compreensão coletiva. Combinar **um** padrão no início — construir o do time ou adotar um existente (ex.: Java Code Conventions).
- Simples vence resistência. Código coletivo ajuda a manter; fora do padrão: avisar, refatorar, publicar a regra duvidosa — às vezes o padrão é que se aproxima do hábito do time.
- Tópicos típicos: mesma tabulação e posição de chaves; caixa consistente; nomes que comunicam (não abreviação conveniente); comentário só quando o código não carrega a intenção (e o comentário evolui com o código).

## Exemplo
Mesma função, dois estilos — o problema é a divergência, não qual chave “ganha”:

```java
public int soma(int a, int b) {
    return a + b;
}
```

## Quando
- **Usar:** time no mesmo código; padrão cedo e simples.
- **Evitar:** estilo pessoal; padrão pesado demais para ser seguido; achar que convenção = [[Padrões de Projeto]].

## Conexões
- [[XP]]
- [[Programação em Pares]]
- [[Integridade Conceitual]]
- [[Padrões de Projeto]]
- [[Métodos Ágeis de Desenvolvimento de Software]]
