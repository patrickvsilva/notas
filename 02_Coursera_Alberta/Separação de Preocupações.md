Meta-princípio: qualquer **preocupação** (*concern* — o que importa para resolver o problema) deve ser tratada em sua própria seção do design/código, em vez de misturar subproblemas no mesmo módulo.

## Ideia Central
- Preocupações vêm do **espaço do problema** e também da **implementação** (o que representar, manipular, apresentar).
- Processo **contínuo** no design: aplicar [[Abstração]], [[Encapsulamento]], [[Decomposição]] e [[Generalização]]/[[Interface]] para isolar cada preocupação.
- Regra prática: encapsule em uma classe só o que **lhe diz respeito** (ex: `Dog` sabe *comer*; `DogOwner` sabe *obter e dar* a comida).

## Como os 4 princípios ajudam
| Princípio | Papel na separação |
|---|---|
| [[Abstração]] | Isola o conceito relevante do problema |
| [[Encapsulamento]] | Agrupa o pertinente numa classe; separa visão (interface) de implementação ([[Ocultação de Informação]]) |
| [[Decomposição]] | Parte o todo em classes/componentes com responsabilidades distintas |
| [[Generalização]] / [[Interface]] | Extrai contratos comuns sem misturar implementações |

## Exemplo (`SmartPhone`)
- **Antes:** uma classe com câmera + telefone → baixa [[Coesão]]; troca a câmera exige editar a classe inteira.
- **Depois:**
  - `Camera` / `Phone` como [[Interface|interfaces]] + classes que as implementam;
  - `SmartPhone` **coordena** e *encaminha* chamadas às partes (não implementa o detalhe);
  - construtor recebe as interfaces; **quem instancia** câmera/telefone é outra responsabilidade.
- Resultado: ↑ [[Coesão]] e [[Modularidade]]; trade-off → ↑ [[Acoplamento]] (o coordenador depende das interfaces). Ver [[Complexidade de Design]].

```java
public class SmartPhone {
    private Camera camera;
    private Phone phone;

    public SmartPhone(Camera camera, Phone phone) {
        this.camera = camera;
        this.phone = phone;
    }

    public void takePhoto() { camera.capture(); }
    public void call(String number) { phone.dial(number); }
}
```

## Meta
Código flexível, reutilizável e manutenível: cada classe contém só o necessário para o seu trabalho; partes trocáveis sem reescrever o sistema.

## Quando
- **Usar:** para isolar cada preocupação e ganhar [[Modularidade]] / alta [[Coesão]].
- **Evitar:** fragmentar demais (overengineering) ou criar dependências só por separar.

## Conexões
- [[Design Orientado a Objetos]]
- [[Modularidade]]
- [[Complexidade de Design]]
- [[Coesão]]
- [[Acoplamento]]
- [[Decomposição]]
- [[Encapsulamento]]
- [[Ocultação de Informação]]
- [[Abstração]]
- [[Generalização]]
- [[Interface]]
- [[Objetos de Controle]]
- [[Arquitetura de Software]]
