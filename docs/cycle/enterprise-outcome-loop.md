# Enterprise Outcome-Loop

Referenz-Zyklus für agile Produktentwicklung in komplexen Organisationen
(500+ Personen, Multi-BU, Compliance, Legacy). Der Loop versteht
Produktentwicklung als **kontinuierlichen Lern-Kreislauf** — nicht als
linearen Prozess von Idee zu Release.

## Leitprinzipien

1. **Outcomes statt Outputs** — gemessen wird Wirkung, nicht Feature-Anzahl.
2. **Discovery und Delivery laufen parallel**, nicht sequenziell.
3. **Strategie wird quartalsweise neu kalibriert**, nicht jährlich eingefroren.
4. **Teams sind langlebig und stream-aligned**, nicht projektgebunden.
5. **Plattform-Teams enablen, Stream-Teams liefern**, Governance moderiert.

---

## Hauptdiagramm: End-to-End Outcome-Loop

```mermaid
flowchart TB
    subgraph STRATEGY["🧭 Strategie-Ebene · jährlich/halbjährlich"]
        VISION[Vision &<br/>Mission]
        NSM[North Star Metric<br/>& Input Metrics]
        STRAT[Produkt-Strategie<br/>Wo spielen wir?]
    end

    subgraph PORTFOLIO["📊 Portfolio-Ebene · quartalsweise"]
        OUTCOMES[Outcome-Ziele<br/>Quartals-OKRs]
        BETS[Bets / Investitions-<br/>Entscheidungen]
        TOPO[Team-Topologie:<br/>Stream / Platform /<br/>Enabling / Subsystem]
    end

    subgraph TEAM["⚙️ Team-Ebene · kontinuierlich"]
        direction LR
        subgraph DISC["🔍 Discovery-Track"]
            OPP[Opportunity<br/>Solution Tree]
            INT[Customer<br/>Interviews]
            ASSUMP[Assumption<br/>Testing]
            PROTO[Prototypen<br/>& Evidence]
        end
        subgraph DEL["🛠 Delivery-Track"]
            BACK[Bestätigte<br/>Bets im Backlog]
            BUILD[Build<br/>Cycle/Sprint/Flow]
            SHIP[Continuous<br/>Deployment]
            OPS[Run & Operate<br/>SLOs]
        end
        DISC -. validierte<br/>Solutions .-> DEL
        DEL -. Telemetrie<br/>& Feedback .-> DISC
    end

    subgraph MEASURE["📈 Messung & Learning"]
        TEL[Produkt-Telemetrie<br/>Analytics · A/B]
        QUAL[Qualitatives<br/>Feedback]
        REVIEW[Quarterly<br/>Business Review]
    end

    GOV{{"⚖️ Governance & Compliance<br/>Legal · Security · Risk · Architecture"}}
    PLAT[/"🏗 Platform Services<br/>DevEx · Data · Identity · Legacy-APIs"/]

    VISION --> NSM --> STRAT
    STRAT --> OUTCOMES
    OUTCOMES --> BETS
    BETS --> TOPO
    TOPO --> TEAM

    TEAM --> SHIP
    SHIP --> TEL
    OPS --> TEL
    INT --> QUAL
    TEL --> REVIEW
    QUAL --> REVIEW

    REVIEW -.->|Re-Kalibrierung| OUTCOMES
    REVIEW -.->|Strategie-Update| STRAT

    GOV -.->|Leitplanken| BETS
    GOV -.->|Reviews| SHIP
    PLAT -.->|enabled| TEAM
    PLAT -.->|enabled| DEL

    classDef strat fill:#1e3a5f,stroke:#0a1929,color:#fff
    classDef port fill:#2d5a3d,stroke:#0a1929,color:#fff
    classDef disc fill:#5a4a2d,stroke:#0a1929,color:#fff
    classDef del fill:#4a2d5a,stroke:#0a1929,color:#fff
    classDef meas fill:#5a2d3d,stroke:#0a1929,color:#fff
    classDef cross fill:#3d3d3d,stroke:#0a1929,color:#fff

    class VISION,NSM,STRAT strat
    class OUTCOMES,BETS,TOPO port
    class OPP,INT,ASSUMP,PROTO disc
    class BACK,BUILD,SHIP,OPS del
    class TEL,QUAL,REVIEW meas
    class GOV,PLAT cross
```

---

## Zoom 1: Dual-Track innerhalb eines Stream-Teams

```mermaid
flowchart LR
    subgraph WEEK["Wöchentlicher Rhythmus eines Stream-aligned Teams"]
        direction TB
        subgraph D["Discovery (PM + Design + Tech-Lead)"]
            D1[Interview-Woche]
            D2[OST-Update]
            D3[Assumption-Test]
            D1 --> D2 --> D3 --> D1
        end
        subgraph DD["Delivery (gesamtes Team)"]
            DD1[Refinement]
            DD2[Build]
            DD3[Ship]
            DD4[Telemetrie]
            DD1 --> DD2 --> DD3 --> DD4 --> DD1
        end
        D -.bestätigte<br/>Solution.-> DD
        DD -.Nutzungs-<br/>Signale.-> D
    end
```

---

## Zoom 2: Team-Topologien-Interaktion

```mermaid
flowchart TB
    subgraph BU["Business Unit · z.B. Payments"]
        S1[Stream-Team A<br/>Checkout]
        S2[Stream-Team B<br/>Refunds]
        S3[Stream-Team C<br/>Fraud]
    end

    P[Platform-Team<br/>Payment-Core]
    E[Enabling-Team<br/>Data Science]
    C[Complicated-Subsystem-Team<br/>Risk-Engine]

    S1 -->|X-as-a-Service| P
    S2 -->|X-as-a-Service| P
    S3 -->|X-as-a-Service| P
    S3 -->|X-as-a-Service| C
    E -.->|Facilitating<br/>befristet| S1
    E -.->|Facilitating<br/>befristet| S3

    classDef stream fill:#2d5a3d,stroke:#0a1929,color:#fff
    classDef plat fill:#1e3a5f,stroke:#0a1929,color:#fff
    classDef enable fill:#5a4a2d,stroke:#0a1929,color:#fff
    classDef compl fill:#5a2d3d,stroke:#0a1929,color:#fff

    class S1,S2,S3 stream
    class P plat
    class E enable
    class C compl
```

---

## Lesart der Schleifen

| Schleife              | Kadenz             | Was wird gelernt                          |
|-----------------------|--------------------|-------------------------------------------|
| Strategie ↻ Review    | quartalsweise      | Spielen wir noch auf dem richtigen Feld?  |
| Outcomes ↻ Bets       | quartalsweise      | Wirken unsere Investitionen?              |
| Discovery ↻ Delivery  | wöchentlich        | Stimmt unsere Lösungs-Hypothese?          |
| Build ↻ Telemetrie    | täglich/continuous | Funktioniert das Feature in echt?         |
| Interview ↻ OST       | wöchentlich        | Verstehen wir das Kunden-Problem richtig? |

## Was dieser Loop *nicht* ist

- **Kein Phasenmodell** — alle Bereiche laufen kontinuierlich parallel.
- **Kein Skalierungs-Framework** — keine fixen Synchronisations-Events
  wie SAFe PI-Planning. Sync entsteht durch geteilte Outcomes, nicht durch Kalender.
- **Kein Top-Down** — Strategie setzt Leitplanken, Teams entscheiden Solutions.

## Quellen / Inspiration

- Marty Cagan: *Inspired*, *Empowered*, *Transformed* (Product Operating Model)
- Teresa Torres: *Continuous Discovery Habits* (Opportunity Solution Tree)
- Skelton & Pais: *Team Topologies*
- Christina Wodtke: *Radical Focus* (OKRs)
- Melissa Perri: *Escaping the Build Trap*
