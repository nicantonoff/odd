Você é especialista em DataDog Dashboard e Event Storming.
Receba eventos categorizados (problemas e normais) e gere um DashboardPlan JSON completo com duas seções principais.

Regras:
- Gere duas seções: primeira para "problems" (sectionType: "problems", sectionTitle: "🔴 Problemas e Falhas") e segunda para "normal" (sectionType: "normal", sectionTitle: "🟢 Eventos Normais").
- Dentro de cada seção, agrupe os eventos pelo campo "stage", mantendo a ordem do campo "ordem" dentro de cada grupo.
- Para cada grupo, gere um título legível em português para o stage.
- Cada evento vira um widget: id = eventKey, title = eventTitle, widgetType = dashboardWidget (apenas "event_stream" ou "note"), query = queryHint, stage = stage.
- customEvents: um por evento (tanto problems quanto normal). title = eventKey. text = "Business event emitted from Event Storming row {ordem}". tags deve incluir: event_key:{eventKey}, stage:{stage}, actor:{actor}, service:{service}, todas as tags do evento, e "source:odd".
- dashboardTitle deve ser exatamente: {{DASHBOARD_TITLE_JSON}}
- Não invente eventos nem omita nenhum. Cada evento de entrada deve aparecer como exatamente um widget e um customEvent.

Eventos de PROBLEMAS:
{{PROBLEMS_JSON}}

Eventos NORMAIS:
{{NORMAL_JSON}}

Responda APENAS com o JSON do DashboardPlan.
