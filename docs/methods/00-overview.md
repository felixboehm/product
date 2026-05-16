# Methoden-Übersicht

Drei Cluster werden hier verglichen — bewusst *ohne* Skalierungs-Frameworks
(SAFe/LeSS/Nexus). Die Auswahl folgt der These, dass moderne Enterprise-Orgs
Komplexität besser über **Outcome-Steuerung + Team-Topologien + Discovery-Kultur**
beherrschen als über zentral choreographierte Sync-Events.

→ Vergleichsmatrix: [comparison/matrix.md](../comparison/matrix.md)

## Cluster A — Klassisch (Team-Level)

| Methode                | Kernidee                                                   |
|------------------------|------------------------------------------------------------|
| [Scrum](classical/scrum.md)     | Zeitlich getakteter empirischer Prozess, fixe Rollen       |
| [Kanban](classical/kanban.md)   | Flow-Optimierung, WIP-Limits, kontinuierliche Lieferung    |
| [XP](classical/xp.md)           | Engineering-Disziplin: TDD, Pair, CI, Refactor             |
| [Crystal](classical/crystal.md) | Adaptive Methoden-Familie nach Team-Größe und Kritikalität |

## Cluster B — Discovery / Produkt-orientiert

| Methode                                                       | Kernidee                                                |
|---------------------------------------------------------------|---------------------------------------------------------|
| [Shape Up](discovery/shape-up.md)                             | 6-wöchige Zyklen, geformte Pitches, betting table       |
| [Dual-Track Agile](discovery/dual-track-agile.md)             | Discovery und Delivery parallel im selben Team          |
| [Continuous Discovery](discovery/continuous-discovery.md)     | Wöchentliche Kunden-Kontakte, Opportunity Solution Tree |
| [Lean Startup](discovery/lean-startup.md)                     | Build-Measure-Learn, validiertes Lernen, Pivot          |
| [Jobs-to-be-Done](discovery/jtbd.md)                          | Kundensicht über "Jobs", die sie erledigen wollen       |

## Cluster C — Modern / Trend (2025-2026)

| Methode                                                            | Kernidee                                              |
|--------------------------------------------------------------------|-------------------------------------------------------|
| [Team Topologies](modern/team-topologies.md)                       | 4 Team-Typen + 3 Interaktionsmodi                     |
| [FAST Agile](modern/fast-agile.md)                                 | Fluid teams, frequent self-selection, marketplace     |
| [Outcome-based Roadmapping](modern/outcome-roadmapping.md)         | Roadmap als Outcome-Hypothesen, nicht Feature-Liste   |
| [Product Operating Model](modern/product-operating-model.md)       | Empowered Teams, Outcomes, Coaching (Cagan)           |
| [AI-augmented Workflows](modern/ai-augmented-workflows.md)         | LLMs in Discovery, Spec-Writing, Code, QA, Research   |

## Wie diese Methoden zusammenspielen

Sie sind **nicht** alternativ zu lesen. In einer reifen Enterprise-Produktorg
wirken typischerweise zusammen:

- **Org-Design:** Team Topologies
- **Operating Model:** Product Operating Model
- **Strategie-Visualisierung:** Outcome-based Roadmapping
- **Discovery-Praxis:** Continuous Discovery + Dual-Track Agile + JTBD
- **0→1-Bets:** Lean Startup
- **Delivery-Engine (Stream-Teams):** Scrum oder Shape Up
- **Delivery-Engine (Platform-Teams):** Kanban
- **Engineering-Fundament:** XP-Praktiken (TDD, CI, Pair, Refactor)
- **Querschnitts-Beschleuniger:** AI-augmented Workflows

Crystal und FAST sind eher ideengeschichtlich relevant —
ihre *Konzepte* (Größen-Sensitivität, Selbst-Selektion) prägen
heutige Praxis, in Reinform aber selten adoptiert.
