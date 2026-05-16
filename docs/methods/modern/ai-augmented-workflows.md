# AI-augmented Product Workflows

## Kernidee

Generative KI (vor allem LLMs) durchzieht den gesamten
Produktentwicklungs-Zyklus als **Querschnitts-Beschleuniger**:
Research-Synthese, Spec-Writing, Code-Generation, Test-Erstellung,
Telemetrie-Analyse, Kommunikation. Keine eigenständige Methode,
sondern eine Layer-Veränderung *aller* Methoden.

## Herkunft & Vordenker

Keine einzelne Quelle — emergent ab 2023 mit GPT-4, ab 2025 mit
Sonnet/Opus 4-Familie und Agent-Frameworks (Claude Code, Cursor,
Devin, Cognition, OpenAI Codex). Vordenker im Produkt-Bereich:
Lenny Rachitsky, Aakash Gupta, Marty Cagan (kritisch), Jakob Nielsen.

## Zentrale Artefakte / Rituale / Rollen

**Pro Phase:**
- **Discovery:** automatisierte Interview-Transkription + Coding,
  Survey-Generierung, Persona-Validierung mit synthetischen Nutzern
  (vorsichtig), Insights-Cluster
- **Strategie/Roadmap:** Spec-Drafts, Outcome-Hypothesen-Generierung,
  Competitive Analysis
- **Delivery:** AI-Coding-Assistants (Claude Code, Cursor), Spec-zu-Code,
  Test-Generierung, Code-Review-Assistance
- **Operate:** Log-/Telemetrie-Analyse, On-Call-Assistance, Incident-Summaries
- **Querschnitt:** Meeting-Summaries, Stakeholder-Updates, Doku

**Neue Rollen (entstehend):** AI Product Engineer, Prompt/Context Engineer,
AI Governance Officer

## Kadenz

Kontinuierlich, prompt-getrieben. Kein eigenes Ritual — verändert
bestehende Rituale.

## Stärken

- 2–10× Beschleunigung in bestimmten Tasks (Doku, Code-Boilerplate,
  Research-Synthese)
- Senkt Einstiegshürde für neue Domänen
- Macht Discovery-Methoden skalierbar (mehr Interviews pro PM)
- Erlaubt schnellere Prototypen-Iteration

## Schwächen / Anti-Patterns

- **Hallucination-Risiko** — vor allem in Strategie und Research
- **Output-Inflation:** mehr Specs ≠ bessere Produkte
- **"Vibe Coding":** schneller Code ohne Verständnis erzeugt unwartbare Systeme
- **Synthetic Users** ersetzen keine echten Kunden (Cagan-Kritik)
- **Compliance/Privacy:** Kunden-Daten in fremde Modelle
- **Skill-Atrophie** wenn nur noch generiert, nicht mehr begründet wird

## Enterprise-Eignung (500+)

Aktuell rapide Adoption. Kritische Themen:
- **Modell-Auswahl & Hoheit** (Cloud-Provider, lokale Modelle, EU AI Act)
- **Governance** (PII, IP, Audit-Trails)
- **Skill-Building** vs. Tool-Abhängigkeit

## Verhältnis zum Outcome-Loop

**Querschnitts-Layer** über *allen* Ebenen des Hauptdiagramms.
Eigene Visualisierung sinnvoll — als nächste Iteration des Repos.

## Quellen

- Rachitsky: "Lenny's Newsletter" (lennysnewsletter.com)
- Nielsen Norman Group: AI-UX-Research (nngroup.com)
- Anthropic Engineering Blog (claude.com/engineering)
- Cagan: "AI and the Product Operating Model" (svpg.com, 2024)
- EU AI Act, Risk Tiers für Produkt-Anwendungen
