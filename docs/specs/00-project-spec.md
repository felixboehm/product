# Spec 00: Projekt-Scope und Design-Entscheidungen

**Status:** Draft
**Datum:** 2026-05-16

## Problemstellung

Agile Produktentwicklung im Enterprise-Kontext ist methodisch fragmentiert.
Klassische Frameworks (Scrum/Kanban) lösen Team-Level-Probleme, aber nicht
Outcome-Steuerung, Discovery-Qualität und Cross-Team-Koordination im großen Maßstab.
Skalierungs-Frameworks (SAFe, LeSS) füllen diese Lücke, sind aber prozesslastig
und stehen in der Kritik der modernen Produkt-Community (Cagan, Skelton, Torres).

Dieses Repo dokumentiert eine *Alternative*: den modernen
Product-Operating-Model-Stack als Antwort auf Enterprise-Komplexität,
ergänzt um klassische Team-Methoden und Discovery-Praktiken.

## Scope

**In Scope:**
- Klassische agile Frameworks: Scrum, Kanban, XP, Crystal
- Discovery/Produkt-orientierte Methoden: Shape Up, Dual-Track Agile,
  Continuous Discovery (Torres), Lean Startup, Jobs-to-be-Done
- Moderne/Trend-Ansätze (2025/26): Team Topologies, FAST Agile,
  Outcome-based Roadmapping, Product Operating Model (Cagan),
  AI-augmented Product Workflows
- Zentrales Visualisierungs-Artefakt: End-to-End Outcome-Loop für Enterprise (500+)

**Out of Scope (bewusst):**
- SAFe, LeSS, Nexus, Scrum@Scale, Disciplined Agile, Spotify-Modell
- Detaillierte Tool-Vergleiche (Jira/Linear/...) — Fokus liegt auf Methoden
- Konkrete Org-Implementierungs-Playbooks

## Output-Form

- **Format:** Markdown mit eingebetteten Mermaid-Diagrammen
- **Versionierung:** Git, semantische Commits (feat/fix/docs/refactor/chore)
- **Workflow:** PR-basiert, keine direkten Pushes auf main
- **Detail-Tiefe pro Methode:** einheitliches Profil-Template (siehe unten)

## Methoden-Profil-Template

Jede Methode wird nach demselben Schema dokumentiert:

```
## Kernidee (2-3 Sätze)
## Herkunft & Vordenker
## Zentrale Artefakte / Rituale / Rollen
## Kadenz (Zyklus-Länge)
## Stärken
## Schwächen / Anti-Patterns
## Enterprise-Eignung (500+)
## Verhältnis zum Outcome-Loop
## Quellen
```

## Erfolgs­kriterium

Eine Produkt-Person aus einer Enterprise-Org kann das Repo lesen und:

1. den modernen Outcome-Loop *als Bild* erfassen (Hauptdiagramm),
2. fundiert begründen, *warum* der POM-Stack als Alternative zu SAFe trägt,
3. einzelne Methoden im Profil-Format vergleichen.

## Offene Fragen

- Pro Methode: nur Profil oder zusätzlich eigenes Sub-Diagramm?
- Vergleichsmatrix: Spalten-Achsen festlegen (Kadenz, Discovery-Anteil,
  Outcome-Orientierung, Team-Autonomie, Enterprise-Reife, ...)
- Soll AI-augmented eine eigene Methode sein oder Querschnitts-Layer?
