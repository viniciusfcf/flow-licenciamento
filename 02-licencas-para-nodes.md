# 2. Licenças → Nodes

> **Pergunta:** cada licença dá direito de usar quais *nodes*? (inverso do [documento 1](01-nodes-para-licencas.md))

Legenda: ✅ disponível · ⭐ somente Advanced · 🟡 parcial · ❌ não disponível.

---

## Família A · Marketing Cloud Next — tier **Growth**

*Verbatim:* "Salesforce Enterprise and Unlimited Editions with Marketing Cloud Next **Growth** Edition …"

**Tipos de Flow liberados:** todos os 5 — Activation-Triggered, Automation Event-Triggered, Broadcast, On-Demand, Audience (e a variante Segment-Triggered).

**Elementos de canvas liberados:** todos os elementos, **exceto** `Path Experiment`.

- Assignment, Collection Filter, Collection Sort, Create Consent, Create Records, Decision,
  Delete Records, Get Records, Loop, Send Email Message, Send Mobile App Message,
  Send Mobile In-App Message, Send SMS Message, Send RCS Message, Send to Journey,
  Subflow, Transform, Update Records, Wait for Conditions, Wait Until Date, Wait for Amount of Time.
- ❌ **`Path Experiment`** — não disponível no Growth.

---

## Família A · Marketing Cloud Next — tier **Advanced**

*Verbatim:* "Salesforce Enterprise and Unlimited Editions with Marketing Cloud Next … **Advanced** Edition"

**Superconjunto do Growth.** Tudo o que o Growth libera, **mais**:

- ⭐ **`Path Experiment`** (elemento de canvas) — até 10 versões de experiência A/B/N.

**Tipos de Flow liberados:** todos os 5 (iguais ao Growth).

**Elementos de canvas liberados:** **todos**, incluindo `Path Experiment`.

> `Path Experiment` como **elemento** exige Advanced. A **feature** de experimentação
> (*Path Experiments*) exige adicionalmente **Personalization** — ver [documento 4](04-licencas-para-features.md).

---

## Família B · Marketing Cloud Engagement (Pro+, Corporate+, Enterprise+)

*Verbatim:* "Marketing Cloud Engagement **Pro+**, **Corporate+**, and **Enterprise+** Editions"

**Tipos de Flow liberados:** todos os 5 tipos de flow de marketing são listados como disponíveis nesta família.

**Elementos de canvas:** a página de referência de elementos documenta a matriz de disponibilidade
sob a **Família A** (Enterprise/Unlimited + Growth/Advanced). Para esta família, valide no help e no
provisionamento da org quais elementos de envio/lógica estão habilitados no seu pacote específico
(Pro+ × Corporate+ × Enterprise+).

---

## Quadro-resumo (tipos de flow por licença)

| Tipo de Flow | A · Growth | A · Advanced | B · MC Engagement |
|--------------|:----------:|:------------:|:-----------------:|
| Activation-Triggered | ✅ | ✅ | ✅ |
| Automation Event-Triggered | ✅ | ✅ | ✅ |
| Broadcast | ✅ | ✅ | ✅ |
| On-Demand | ✅ | ✅ | ✅ |
| Audience (+ Segment-Triggered) | ✅ | ✅ | ✅ |

## Quadro-resumo (elementos por tier da Família A)

| Elemento | A · Growth | A · Advanced |
|----------|:----------:|:------------:|
| `Path Experiment` | ❌ | ⭐ ✅ |
| Todos os demais elementos | ✅ | ✅ |

---

### Fontes
- [Compare Flow Types — `mktg.mktg_flow_types_compare.htm`](https://help.salesforce.com/s/articleView?id=mktg.mktg_flow_types_compare.htm&type=5)
- [Flow Builder Features and Elements for Marketers — `mktg.mktg_flow_elements_reference.htm`](https://help.salesforce.com/s/articleView?id=mktg.mktg_flow_elements_reference.htm&type=5)
