# Licenciamento de Flow — Marketing Cloud Next & Marketing Cloud Engagement

> ⚠️ **Documento gerado com IA em 2026-07-21.** Pode conter erros ou desatualizações —
> valide as informações críticas diretamente nas fontes oficiais antes de usar para decisão
> de compra ou implementação.
>
> **Fontes utilizadas (help.salesforce.com):**
> - [Compare Flow Types — `mktg.mktg_flow_types_compare.htm`](https://help.salesforce.com/s/articleView?id=mktg.mktg_flow_types_compare.htm&type=5)
> - [Flow Builder Features and Elements for Marketers — `mktg.mktg_flow_elements_reference.htm`](https://help.salesforce.com/s/articleView?id=mktg.mktg_flow_elements_reference.htm&type=5)
> - [Marketing Cloud (hub) — `mktg.mktg_main.htm`](https://help.salesforce.com/s/articleView?id=mktg.mktg_main.htm&type=5)

Conjunto de mapeamentos que respondem a duas perguntas:

1. **Licenciamento dos elementos do Flow** — quais *nodes* (tipos de flow + elementos de canvas) existem e em que licença cada um é liberado.
2. **Features de plataforma por licença de marketing** — o que cada licença nova de marketing (Marketing Cloud Next **Growth** / **Advanced**) adiciona à plataforma.

## Documentos

| # | Documento | Pergunta que responde |
|---|-----------|-----------------------|
| 1 | [01-nodes-para-licencas.md](01-nodes-para-licencas.md) | Quais **nodes** existem e **em que licenças** cada um pode ser usado |
| 2 | [02-licencas-para-nodes.md](02-licencas-para-nodes.md) | Cada **licença** e **quais nodes** ela dá direito de usar (inverso do #1) |
| 3 | [03-features-para-licencas.md](03-features-para-licencas.md) | Quais **features** existem e **em que licenças** cada uma é liberada |
| 4 | [04-licencas-para-features.md](04-licencas-para-features.md) | Cada **licença** e **quais features** ela dá direito de usar (inverso do #3) |

## Convenção de licenças usada em todos os documentos

O help da Salesforce descreve **duas famílias de licença** que habilitam os flows de marketing:

| Sigla | Família de licença | Texto "Required Editions" (verbatim) |
|-------|--------------------|--------------------------------------|
| **A** | Marketing Cloud Next (sobre o Core CRM) | *"Salesforce Enterprise and Unlimited Editions with Marketing Cloud Next **Growth** Edition or **Advanced** Edition"* |
| **B** | Marketing Cloud Engagement | *"Marketing Cloud Engagement **Pro+**, **Corporate+**, and **Enterprise+** Editions"* |

Dentro da Família **A** há dois tiers, e é a diferença entre eles que importa para as features:

| Tier | O que é |
|------|---------|
| **A · Growth** | Tier de entrada do Marketing Cloud Next. |
| **A · Advanced** | Superconjunto do Growth; adiciona *On-Canvas Insights*, *Path Experiments* (elemento + feature) e experimentação A/B/N. |

> **Observação importante:** a página de *comparação de tipos de flow* lista **as duas famílias (A e B)**.
> Já a página de referência de **elementos e features de flow** documenta o comportamento sob a
> **Família A (Enterprise/Unlimited + Growth/Advanced)**. Onde há distinção de tier (Growth × Advanced),
> ela está sinalizada em cada documento.

## Legenda

- ✅ Disponível
- ⭐ **Somente Advanced** (dentro da Família A)
- ➕ Requer complemento adicional (ex.: Personalization)
- 🟡 Disponível parcialmente (comportamento reduzido)
- ❌ Não disponível

## Fontes (help.salesforce.com)

- [Compare Flow Types — `mktg.mktg_flow_types_compare.htm`](https://help.salesforce.com/s/articleView?id=mktg.mktg_flow_types_compare.htm&type=5)
- [Flow Builder Features and Elements for Marketers — `mktg.mktg_flow_elements_reference.htm`](https://help.salesforce.com/s/articleView?id=mktg.mktg_flow_elements_reference.htm&type=5)
- [Marketing Cloud (hub) — `mktg.mktg_main.htm`](https://help.salesforce.com/s/articleView?id=mktg.mktg_main.htm&type=5)

> Coletado em 2026-07-21. As páginas de detalhe de cada elemento vivem no namespace `platform.*`
> (ex.: `platform.flow_ref_elements_path_experiment.htm`); a tabela-fonte deste conjunto é a
> `mktg.mktg_flow_elements_reference.htm`, que é autoritativa para disponibilidade por edição.
