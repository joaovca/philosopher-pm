# Philosopher PM

Skills para investigar decisões de produto, preparar refinamentos com engenharia e avaliar negócios baseados em IA.

| Skill | Quando usar |
| --- | --- |
| [socratic-prd](.agents/skills/socratic-prd/SKILL.md) | Investigar o resultado desejado, a prova de sucesso e a relação causal com a solução proposta. |
| [product-refinement](.agents/skills/product-refinement/SKILL.md) | Transformar demandas de produto em rascunhos para refinamento com engenharia. |
| [oaas-strategy](.agents/skills/oaas-strategy/SKILL.md) | Avaliar negócios de AI-enabled services / Outcomes as a Service em oito critérios, com total de 40 pontos. |

Abra este repositório no Codex e invoque a skill pelo nome, acompanhada do contexto da sua demanda. Exemplos:

```text
$socratic-prd Quero investigar se esta funcionalidade resolve o problema dos clientes: ...

$product-refinement Prepare esta demanda para refinamento com engenharia: ...

$oaas-strategy Avalie esta ideia: [ideia, cliente, problema e modelo de receita].
```

As skills ficam em `.agents/skills/`. `product-refinement` e `socratic-prd` são cópias locais completas, incluindo seus metadados, e podem evoluir independentemente das originais. A skill `oaas-strategy` foi escrita em inglês com base no prompt fornecido.

[AGENTS.md](AGENTS.md) orienta os agentes sobre a escolha dos workflows. Este repositório contém instruções Markdown e não exige instalação de dependências para uso.
