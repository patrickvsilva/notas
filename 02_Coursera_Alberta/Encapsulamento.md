Princípio de design que forma um objeto autocontido ao agrupar dados e comportamentos, expor uma interface pública e restringir o acesso aos detalhes internos.

## Três Ideias
- **Agrupamento:** Atributos (dados) e métodos (comportamentos) que os manipulam ficam juntos na mesma classe.
- **Exposição:** Interface pública pela qual outros objetos usam a classe.
- **Restrição:** Estado e detalhes internos acessíveis apenas de dentro do objeto.

## Relação com Abstração
- [[Abstração]] decide *quais* atributos e comportamentos são relevantes no contexto.
- Encapsulamento garante que essas características fiquem *agrupadas* na mesma classe, com acesso controlado.
- Cada objeto guarda só o que lhe é relevante (ex: Curso conhece seus alunos; Professor conhece suas disciplinas — não a lista completa da universidade).

## Na Prática (design + código)
- No [[Diagrama de Classes]], `-` = privado, `+` = público ([[Visibilidade UML]]).
- Atributos sensíveis ficam privados; o mundo externo passa por métodos aprovados — tipicamente [[Getters e Setters]] (um “portão” que controla *como* e *quando* o dado muda).
- Getters/setters **não** precisam só ler/escrever: podem validar (ex: só muda o curso se GPA > 2.7). O consumidor não vê a regra — só o contrato ([[Pensamento de Caixa Preta]]).

### Exemplo (`Student`)
```
+----------------------------------+
| Student                          |
+----------------------------------+
| - gpa : double                   |
| - degreeProgram : String         |
+----------------------------------+
| + getGpa() : double              |
| + setGpa(gpa : double)           |
| + getDegreeProgram() : String    |
| + setDegreeProgram(p : String)   |
+----------------------------------+
```

```java
public class Student {
    private double gpa;
    private String degreeProgram;

    public double getGpa() { return gpa; }

    public void setGpa(double gpa) {
        if (gpa >= 0 && gpa <= 4.0) this.gpa = gpa;
    }

    public String getDegreeProgram() { return degreeProgram; }

    public void setDegreeProgram(String program) {
        if (gpa > 2.7) this.degreeProgram = program;
    }
}
```

```python
class Student:
    def __init__(self):
        self._gpa = 0.0
        self._degree_program = ""

    def get_gpa(self) -> float:
        return self._gpa

    def set_gpa(self, gpa: float) -> None:
        if 0 <= gpa <= 4.0:
            self._gpa = gpa

    def get_degree_program(self) -> str:
        return self._degree_program

    def set_degree_program(self, program: str) -> None:
        if self._gpa > 2.7:
            self._degree_program = program
```

> Em Python, `_attr` é convenção de “privado” (não há `private` como em Java).

## Benefícios
- **Integridade dos Dados:** Estado só muda via métodos, preservando invariantes e dependências internas.
- **Informação Sensível:** Pode responder consultas derivadas (ex: "em boa situação?") sem revelar o valor bruto (ex: GPA).
- **Mudanças Isoladas:** Interface estável; implementação pode mudar sem afetar consumidores ([[Pensamento de Caixa Preta]], [[Barreira de Abstração]]).
- **Reutilização:** Consumidores precisam só da assinatura dos métodos (entradas, saídas e efeitos).
- **Baixo [[Acoplamento]]:** Conexões óbvias sem “abrir” o módulo (facilidade) — ver [[Complexidade de Design]].

## Conexões
- [[Design Orientado a Objetos]]
- [[Abstração]]
- [[Visibilidade UML]]
- [[Getters e Setters]]
- [[Diagrama de Classes]]
- [[Pensamento de Caixa Preta]]
- [[Barreira de Abstração]]
- [[Complexidade de Design]]
- [[Acoplamento]]
- [[Coesão]]
- [[Decomposição]]
- [[Generalização]]
- [[Tipo Abstrato de Dados]]
