# 4. Licenças → Features

> **Pergunta:** cada licença dá direito de usar quais *features*? (inverso do [documento 3](03-features-para-licencas.md))

Legenda: ✅ disponível · ⭐ somente Advanced · ➕ requer complemento.

---

## Família A · Marketing Cloud Next — tier **Growth**

*Verbatim:* "…with Marketing Cloud Next **Growth** Edition…"

Features de plataforma liberadas:

| Feature | Status |
|---------|:------:|
| **Flow Reports** | ✅ |
| On-Canvas Insights | ❌ (só Advanced) |
| Path Experiments | ❌ (só Advanced ➕ Personalization) |

**Resumo:** o Growth entrega a construção completa de flows (todos os tipos e quase todos os elementos)
+ **Flow Reports**. Não inclui análise on-canvas nem experimentação A/B/N.

---

## Família A · Marketing Cloud Next — tier **Advanced**

*Verbatim:* "…with Marketing Cloud Next … **Advanced** Edition"

**Superconjunto do Growth.** Tudo do Growth, **mais** as features de análise e experimentação:

| Feature | Status |
|---------|:------:|
| **Flow Reports** | ✅ |
| **On-Canvas Insights** | ⭐ ✅ |
| **Path Experiments** | ⭐ ✅ ➕ requer **Personalization** |

**O que o Advanced adiciona em relação ao Growth:**

1. **On-Canvas Insights** — métricas dos flows direto no canvas.
2. **Path Experiments** — testes A/B/N com até 10 versões de experiência (➕ Personalization).
3. **Elemento `Path Experiment`** no canvas (ver [documento 2](02-licencas-para-nodes.md)).

> Exemplo do enunciado original: *"On-Canvas Insights é uma feature disponível com o Marketing Cloud Next Advanced edition."* ✅ Confirmado.

---

## Família B · Marketing Cloud Engagement (Pro+, Corporate+, Enterprise+)

*Verbatim:* "Marketing Cloud Engagement **Pro+**, **Corporate+**, and **Enterprise+** Editions"

Esta família habilita os **tipos de flow** de marketing (ver [documento 2](02-licencas-para-nodes.md)).
As features de plataforma *Flow Reports / On-Canvas Insights / Path Experiments* são documentadas na
página de referência sob a **Família A (Growth/Advanced)**; para MC Engagement, valide no help e no
provisionamento da org qual conjunto de features de flow acompanha o seu pacote.

---

## Quadro-resumo (features por licença)

| Feature | A · Growth | A · Advanced | Requisito extra |
|---------|:----------:|:------------:|-----------------|
| Flow Reports | ✅ | ✅ | — |
| On-Canvas Insights | ❌ | ⭐ ✅ | — |
| Path Experiments | ❌ | ⭐ ✅ | ➕ Personalization |

---

### Fontes
- [Flow Builder Features and Elements for Marketers — `mktg.mktg_flow_elements_reference.htm`](https://help.salesforce.com/s/articleView?id=mktg.mktg_flow_elements_reference.htm&type=5)
- [Marketing Cloud (hub) — `mktg.mktg_main.htm`](https://help.salesforce.com/s/articleView?id=mktg.mktg_main.htm&type=5)
