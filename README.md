<p align="center">
  <img src="Banner.png" width="100%" />
</p>

<h1 align="center">Marcel Buck</h1>

<p align="center">
  <strong>Data Analyst · M.Sc. Wirtschaftsinformatik</strong><br/>
  Python &nbsp;•&nbsp; SQL &nbsp;•&nbsp; Power BI &nbsp;•&nbsp; dbt &nbsp;•&nbsp; DuckDB &nbsp;•&nbsp; Snowflake
</p>

<p align="center">
  <a href="https://linkedin.com/in/marcel-buck-122327233/">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <img src="https://img.shields.io/badge/Status-Offen_für_neue_Rollen-brightgreen?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Standort-Deutschland_·_Remote-blue?style=for-the-badge" />
</p>

---

## Über mich

M.Sc. Wirtschaftsinformatik mit Fokus auf **End-to-End-Datenprojekte** — von der automatisierten Pipeline bis zum Dashboard, das Entscheidungsträger tatsächlich öffnen.

Mein Hintergrund im **Business Development** gibt mir ein Gespür dafür, welche Datenfragen wirklich geschäftskritisch sind — und wie man Ergebnisse so kommuniziert, dass sie auch gehört werden.

- Entwickle und automatisiere **Datenpipelines** (Python · dbt · GitHub Actions)
- Baue **BI-Dashboards** für Entscheidungsträger (Power BI · Tableau)
- Entwickle **ML-Vorhersagemodelle** mit messbarem Ergebnis (ROC-AUC 0.87+)
- Kommuniziere Insights klar — an technische und nicht-technische Stakeholder

---

## Tech Stack

### Analyse & Machine Learning
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas)
![NumPy](https://img.shields.io/badge/Numpy-013243?style=for-the-badge&logo=numpy)
![Scikit-Learn](https://img.shields.io/badge/ScikitLearn-F7931E?style=for-the-badge&logo=scikitlearn)

### Datenbanken & Warehousing
![DuckDB](https://img.shields.io/badge/DuckDB-FDD023?style=for-the-badge&logo=duckdb&logoColor=black)
![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=for-the-badge&logo=snowflake&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

### BI & Visualisierung
![Power BI](https://img.shields.io/badge/PowerBI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![PowerPoint](https://img.shields.io/badge/Tableau-E97627?style=for-the-badge&logo=tableau)
![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoft-excel)

### Data Engineering & Tools
![dbt](https://img.shields.io/badge/dbt-FF694B?style=for-the-badge&logo=dbt&logoColor=white)
[![Tools](https://skillicons.dev/icons?i=git,github,vscode&theme=dark)](https://skillicons.dev)

---

## Projekte

### [Supply-Chain Resilience – End-to-End Projekt](https://github.com/Buck-Data/Supply-Chain-Projekt)

<p align="center">
  <img src="Supply_Chain.png" width="100%" alt="Supply Chain Projekt" />
</p>

| | |
|---|---|
| **Problem** | Lieferkettendaten lagen verteilt und unstrukturiert vor — kein zentrales Bild der Supply-Chain-Lage |
| **Lösung** | Vollautomatisierte End-to-End-Pipeline: Rohdaten → DuckDB Warehouse → dbt → Power BI Dashboard |
| **Impact** | Dashboard aktualisiert sich automatisch — Entscheidungsträger sehen KPIs in Echtzeit |

**Methodik**

- Inkrementelles Laden via State-Tracking — nur neue Datensätze werden verarbeitet
- Parallele Datenabfragen mit 4 Workern (~4x schneller als sequentiell)
- Zweischichtiges dbt-Modell: Staging (Bereinigung) → Sternschema (Dims + Facts)
- 69 automatisierte Datentests (not_null, unique, referentielle Integrität, Geschäftslogik)
- Wöchentliche CI/CD-Pipeline via GitHub Actions

**Wichtige Erkenntnisse**

- Lieferverzögerungen lassen sich auf Engpasslieferanten und kritische Routen zurückführen
- Lagerbestände und Vorlaufzeiten korrelieren messbar mit Saisonalität
- KPI-Tracking pro Lieferant ermöglicht datenbasierte Lieferantensteuerung

`Python` `DuckDB` `dbt Core` `Power BI` `GitHub Actions`

---

### [F1 Analytics – End-to-End Datenpipeline](https://github.com/Buck-Data/F1-End-to-End-Project)

<p align="center">
  <img src="F1_Projekt.png" width="100%" alt="F1 Projekt" />
</p>

| | |
|---|---|
| **Problem** | Formel-1-Renndaten manuell abrufen und auswerten — ineffizient und fehleranfällig |
| **Lösung** | Vollautomatisierte Pipeline: 10 OpenF1-API-Endpunkte → DuckDB Warehouse → dbt → Power BI |
| **Impact** | Dashboard aktualisiert sich automatisch nach jedem Rennwochenende — null manueller Aufwand |

**Methodik**

- Inkrementelles Laden via State-Tracking — nur neue Sessions werden abgerufen
- Parallele API-Abfragen mit 4 Workern (~4x schneller als sequentiell)
- Zweischichtiges dbt-Modell: Staging (Bereinigung) → Sternschema (Dims + Facts)
- 69 automatisierte Datentests (not_null, unique, referentielle Integrität, Geschäftslogik)
- Wöchentliche CI/CD-Pipeline via GitHub Actions (jeden Montag 06:00 UTC)

**Wichtige Erkenntnisse**

- Reifenstrategie und Stint-Längen haben messbaren Einfluss auf Rundenzeiten
- Wetterbedingungen (Temperatur, Luftfeuchtigkeit) korrelieren mit Sektorzeiten
- WM-Standings lassen sich pro Rennen verfolgen und visuell vergleichen

`Python` `DuckDB` `dbt Core` `Power BI` `GitHub Actions`

---

### Kundenabwanderungs-Vorhersage

| | |
|---|---|
| **Problem** | Unternehmen verlieren Kunden, ohne Warnsignale frühzeitig zu erkennen |
| **Lösung** | Klassifikationsmodell in Python zur Vorhersage individuellen Abwanderungsrisikos |
| **Ergebnis** | ROC-AUC: **0.87** |

**Wichtige Erkenntnisse**

- Nutzer mit geringem Engagement kündigen deutlich häufiger
- Preisstufe korreliert stark mit Kündigungen

`Python` `Pandas` `Scikit-Learn` `PostgreSQL`

---

### TDWI 2025 - Student Corner Projekt - AIoT im Wassermanagement

| | |
|---|---|
| **Problem** | Unternehmen verlieren Kunden, ohne Warnsignale frühzeitig zu erkennen |
| **Lösung** | Klassifikationsmodell in Python zur Vorhersage individuellen Abwanderungsrisikos |
| **Ergebnis** | ROC-AUC: **0.87** |

**Wichtige Erkenntnisse**

- Nutzer mit geringem Engagement kündigen deutlich häufiger
- Preisstufe korreliert stark mit Kündigungen

`Python` `Pandas` `Scikit-Learn` `PostgreSQL`

---

### Funnel Analyse (In Bearbeitung)

| | |
|---|---|
| **Problem** | Unternehmen verlieren Kunden, ohne Warnsignale frühzeitig zu erkennen |
| **Lösung** | Klassifikationsmodell in Python zur Vorhersage individuellen Abwanderungsrisikos |
| **Ergebnis** | ROC-AUC: **0.87** |

**Wichtige Erkenntnisse**

- Nutzer mit geringem Engagement kündigen deutlich häufiger
- Preisstufe korreliert stark mit Kündigungen

`Python` `Pandas` `Scikit-Learn` `PostgreSQL`

---

## Berufserfahrung

### Business Development & Process Automation – Werkstudent

- Lead-Recherche-Workflow automatisiert → messbare Zeitersparnis für das Vertriebsteam
- Marktanalysen und Wachstumsstrategien direkt mit Stakeholdern erarbeitet

### Requirements Engineering – Praktikant

- Geschäftsanforderungen strukturiert erhoben und dokumentiert
- Anforderungen in technische Spezifikationen übersetzt
- Als Schnittstelle zwischen Business und Entwicklungsteam agiert

---

## Derzeit am Lernen

`Advanced SQL für Analytics` &nbsp;·&nbsp; `Data Engineering` &nbsp;·&nbsp; `Production ML Pipelines`

---

## Verfügbar für

**Data Analyst · Business Intelligence Analyst · Junior Data Scientist**

📍 Remote · Deutschland · EU

---

## 🤝 Kontakt

<p align="center">
  <a href="https://linkedin.com/in/marcel-buck-122327233/">
    <img src="https://img.shields.io/badge/LinkedIn_–_Marcel_Buck-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  &nbsp;
  <a href="mailto:buckdevelopmentmarcel@gmail.com">
    <img src="https://img.shields.io/badge/E--Mail-D14836?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
</p>
