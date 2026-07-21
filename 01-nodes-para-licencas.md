# 1. Nodes → Licenças

> **Pergunta:** quais *nodes* existem e em que licenças cada um pode ser usado?

No contexto de Flow de marketing, "node" abrange dois níveis:

- **A. Tipos de Flow** — a "casca" da automação (ex.: *Audience Flow*).
- **B. Elementos de Flow** — os blocos que você arrasta no canvas (ex.: *Send Email Message*, *Decision*, *Path Experiment*).

Legenda: ✅ disponível · ⭐ somente **Advanced** · 🟡 parcial · ❌ não disponível · ➕ requer complemento.
Famílias de licença (**A** = MC Next Growth/Advanced · **B** = MC Engagement Pro+/Corporate+/Enterprise+) — ver [README](README.md).

---

## A. Tipos de Flow

Todos os cinco tipos de flow compartilham o mesmo licenciamento — **não há tipo de flow que exija uma edição específica** além das famílias A e B.

| Tipo de Flow | Como é disparado | A · Growth | A · Advanced | B · MC Engagement |
|--------------|------------------|:----------:|:------------:|:-----------------:|
| **Activation-Triggered Flow** | Quando uma ativação é publicada (segue o schedule de publicação do segmento) | ✅ | ✅ | ✅ |
| **Automation Event-Triggered Flow** | Quando ocorre um evento/engagement signal (~15 min) | ✅ | ✅ | ✅ |
| **Broadcast Flow** | Via API, Apex ou por outro flow; audiência dinâmica definida após o start | ✅ | ✅ | ✅ |
| **On-Demand Flow** | Sob demanda via API/Apex para casos de alta prioridade/real-time (transacional) | ✅ | ✅ | ✅ |
| **Audience Flow** | Agendado (uma vez ou recorrente, até de hora em hora) ou imediato; mira segmento/lista/campanha | ✅ | ✅ | ✅ |
| **Segment(-Triggered) Flow** | Variante do Audience Flow que mira membros de segmento (mesmo comportamento de agendamento) | ✅ | ✅ | ✅ |

> Texto verbatim (aplica-se a **todos** os tipos acima):
> *"Available in: Salesforce Enterprise and Unlimited Editions with Marketing Cloud Next Growth Edition or Advanced Edition"*
> *"Available in: Marketing Cloud Engagement Pro+, Corporate+, and Enterprise+ Editions"*

---

## B. Elementos de Flow (nodes de canvas)

Duas dimensões importam para cada elemento:

1. **Em que tipos de flow** o elemento pode ser usado (Audience / Automation Event-Triggered / Activation-Triggered).
2. **Que tier de licença** ele exige. Regra geral: **todos** os elementos estão disponíveis na Família **A (Growth e Advanced)** — **exceto o `Path Experiment`, que é ⭐ somente Advanced**.

| Elemento (node) | O que faz | Em Audience | Em Automation Event | Em Activation | Licença |
|-----------------|-----------|:-----------:|:-------------------:|:-------------:|---------|
| **Assignment** | Define valores em variáveis/coleções | ✅ | ✅ | ✅ | A (Growth+Advanced) |
| **Collection Filter** | Filtra uma coleção por critério gerando outra | ✅ | ✅ | ✅ | A (Growth+Advanced) |
| **Collection Sort** | Reordena/limita itens de uma coleção | ✅ | ✅ | ✅ | A (Growth+Advanced) |
| **Create Consent** | Cria/atualiza status de consentimento de um contact point | ❌ | ✅ | ❌ | A (Growth+Advanced) |
| **Create Records** | Cria registros na org | ✅ | ✅ | ✅ | A (Growth+Advanced) |
| **Decision** | Roteamento IF/ELSE por condições | ✅ | ✅ | ✅ | A (Growth+Advanced) |
| **Delete Records** | Apaga registros permanentemente | ✅ | ✅ | ✅ | A (Growth+Advanced) |
| **Get Records** | Busca registros por filtro e guarda valores | ✅ | ✅ | ✅ | A (Growth+Advanced) |
| **Loop** | Itera sobre itens de uma coleção | ✅ | ✅ | ✅ | A (Growth+Advanced) |
| **Path Experiment** | Até 10 versões de experiência (A/B/N) | ✅ | ✅ | ❌ | ⭐ **A · Advanced apenas** |
| **Send Email Message** | Envia e-mail a membros por condição | ✅ | ✅ | ❌ | A (Growth+Advanced) |
| **Send Mobile App Message** | Envia push notification | ✅ | ✅ | ❌ | A (Growth+Advanced) |
| **Send Mobile In-App Message** | Envia mensagem in-app | ✅ | ✅ | ❌ | A (Growth+Advanced) |
| **Send SMS Message** | Envia SMS aos membros | ✅ | ✅ | ❌ | A (Growth+Advanced) |
| **Send RCS Message** | Envia mensagem RCS | ✅ | ✅ | ❌ | A (Growth+Advanced) |
| **Send to Journey** | Envia membros para uma journey do MC Engagement | ✅ | ✅ | ✅ | A (Growth+Advanced) |
| **Subflow** | Dispara outro flow ativo da org | ✅ | ✅ | ✅ | A (Growth+Advanced) |
| **Transform** | Mapeia/transforma dados de origem → destino | ✅ | ✅ | ✅ | A (Growth+Advanced) |
| **Update Records** | Cria/atualiza registros na org | ✅ | ✅ | ✅ | A (Growth+Advanced) |
| **Wait for Conditions** | Pausa até condições de espera | ✅ | ✅ | 🟡 | A (Growth+Advanced) |
| **Wait Until Date** | Pausa até uma data | ✅ | ✅ | 🟡 | A (Growth+Advanced) |
| **Wait for Amount of Time** | Pausa por um intervalo | ✅ | ✅ | 🟡 | A (Growth+Advanced) |

**Destaques de licenciamento por elemento:**

- ⭐ **`Path Experiment`** é o **único elemento com restrição de tier**: disponível **apenas no Advanced**. (Como *feature* de experimentação, também requer **Personalization** — ver [documento 3](03-features-para-licencas.md).)
- Os elementos de **envio** (`Send Email/SMS/RCS/Mobile App/Mobile In-App`) e o `Path Experiment` **não** funcionam em **Activation-Triggered Flows**.
- `Create Consent` só existe em **Automation Event-Triggered Flows**.
- Os elementos de **Wait** têm suporte 🟡 **parcial** em Activation-Triggered Flows.

---

### Fontes
- [Compare Flow Types — `mktg.mktg_flow_types_compare.htm`](https://help.salesforce.com/s/articleView?id=mktg.mktg_flow_types_compare.htm&type=5)
- [Flow Builder Features and Elements for Marketers — `mktg.mktg_flow_elements_reference.htm`](https://help.salesforce.com/s/articleView?id=mktg.mktg_flow_elements_reference.htm&type=5)
