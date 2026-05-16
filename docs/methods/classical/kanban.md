# Kanban

## Kernidee

Pull-basiertes Flow-System: Arbeit wird visualisiert, WIP limitiert, Fluss
gemessen und kontinuierlich verbessert. Kein Iterations-Rhythmus, keine
fixen Rollen — evolutionärer Ansatz, der die bestehende Organisation
respektiert und schrittweise optimiert.

## Herkunft & Vordenker

David J. Anderson (Microsoft, Corbis, 2007). Wurzeln im Toyota Production
System. Heute Kanban University, Klaus Leopold im DACH-Raum.

## Zentrale Artefakte / Rituale / Rollen

- **Praktiken:** Visualisieren, WIP limitieren, Flow managen, Policies
  explizit machen, Feedback-Loops etablieren, evolutionär verbessern
- **Artefakte:** Kanban-Board, WIP-Limits, Service-Klassen, CFD, Lead-Time-Histogramm
- **Rituale (optional):** Replenishment, Delivery Planning, Service Delivery Review
- **Rollen (optional):** Service Request Manager, Service Delivery Manager

## Kadenz

Kontinuierlich. Cadences (Replenishment, Reviews) typischerweise wöchentlich/14-tägig.

## Stärken

- Minimaler Change-Impact — startet beim Ist-Zustand
- Datenbasiert: Lead Time, Throughput, CFD ersetzen Bauchgefühl
- Skaliert von einem Team bis Portfolio (Flight Levels, Klaus Leopold)
- Ideal für Ops, Platform, Support, gemischte Workloads

## Schwächen / Anti-Patterns

- Wenig Vorgabe zur Priorisierung — kippt zu "wer schreit am lautesten"
- Ohne Service Delivery Review keine echte Verbesserung
- Boards verkommen zu reinen Ticket-Tracker ohne Flow-Management

## Enterprise-Eignung (500+)

Sehr hoch. Besonders stark in Bereichen mit unvorhersehbarer
Nachfrage (Plattform, SRE, Sicherheit). Skaliert über Flight Levels
auf Portfolio-Ebene.

## Verhältnis zum Outcome-Loop

Ideale **Delivery-Track**-Engine, vor allem für Platform-Teams im
[[team-topologies]]-Modell. Lässt sich nahtlos mit [[continuous-discovery]] koppeln.

## Quellen

- Anderson: *Kanban: Successful Evolutionary Change*
- Leopold: *Rethinking Agile*, *Flight Levels*
- kanban.university
