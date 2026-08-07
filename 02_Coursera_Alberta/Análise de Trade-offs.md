Processo essencial na [[Arquitetura de Software]] para equilibrar atributos de qualidade concorrentes e restrições de negócio.

> 💡 *"A qualidade é o principal trabalho do arquiteto: definir o que é qualidade e advogar por ela equilibrando 'Tempo de Mercado' vs 'Perfeição de Código'."*

## Trade-offs Clássicos no Desenvolvimento

| Conflito | Descrição do Trade-off | Consequência da Falta de Balanço |
| :--- | :--- | :--- |
| **[[Desempenho]] vs [[Manutenibilidade]]** | Código ultra-otimizado costuma ser menos legível e modular. | Perda de velocidade de manutenção futura. |
| **[[Segurança]] vs [[Desempenho]] / Conveniência** | Checagens extras e criptografia adicionam overhead e etapas ao usuário. | Experiência ruim (análogo a colocar 10 trancas na porta da casa). |
| **Qualidade Técnica vs Time-to-Market** | Engenheiros buscam 100% de cobertura; o negócio precisa lançar e faturar. | Atraso de lançamento ou acúmulo de [[Débito Técnico]]. |
| **Compatibilidade Reversa vs Desempenho** | Código legado suporte piora desempenho e clareza. | Complexidade desnecessária na base de código. |

## Mitigação e Boas Práticas
1. **Definição de Guardrails (Limites):** Estabelecer o que é *não-negociável* e o que é *negociável*.
2. **Contexto do Domínio:** Exigências mudam conforme o contexto (ex: casa em bairro de alta criminalidade vs baixa criminalidade).
3. **Perspectivas Múltiplas & Reviews:** Evitar consequências não intencionais fazendo sessões de *Design Review* com múltiplos perfis (devs, segurança, stakeholders).
4. **Prototipagem & Testes:** Testar decisões precocemente (ex: simulação de evacuação de incêndio em casa com grades nas janelas).

## Conexões
- [[Arquitetura de Software]]
- [[Atributos de Qualidade]]
- [[Requisitos Não-Funcionais]]
