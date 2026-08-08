Relação *has-a* **fraca** da [[Decomposição]]: o todo tem partes que lhe pertencem, mas as partes (e o todo) podem existir independentemente — compartilhamento entre vários todos é possível.

## Sinais
- O todo “tem” a parte (ex: lista de crew no airliner).
- Sem a parte o todo ainda existe (avião sem tripulação ainda é avião).
- A parte sobrevive fora do todo (tripulação existe fora do voo).

## UML
Diamante **vazio** (◇) no lado do **todo**.

```
Airliner ◇── 0..* Crew
CourseSection ◇── 0..* Student
PetStore ◇── 0..* Pet
```

## Código (tem, mas lifetimes independentes)
```java
public class Airliner {
    private List<Crew> crew = new ArrayList<>();

    public void addCrew(Crew member) {
        crew.add(member);
    }
}
```

O `Crew` é criado fora e adicionado; não nasce nem morre com o `Airliner`.

## Quando
- **Usar:** *has-a* fraco com lifetimes independentes e partes compartilháveis.
- **Evitar:** se a parte morre com o todo — use [[Composição]].

## Conexões
- [[Decomposição]]
- [[Associação]]
- [[Composição]]
- [[Cardinalidade UML]]
- [[Diagrama de Classes]]
