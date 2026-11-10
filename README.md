# Digitaler Ratenkredit – Hansebank

Anforderungsanalyse für die Digitalisierung des Ratenkreditprozesses einer fiktiven Regionalbank – von der Ausgangslage über Prozess- und Customer-Journey-Analyse bis zu umsetzungsreifen User Stories und KPI-Auswertungen.

## Ausgangslage

Die Hansebank vergibt Ratenkredite an Privatkunden heute fast ausschließlich über die Filiale:

- Der Kunde vereinbart einen Termin und füllt einen Papierantrag aus.
- Einkommensnachweise werden kopiert und manuell erfasst.
- Die SCHUFA-Abfrage und die Bonitätsprüfung stoßen Sachbearbeiter manuell an.
- Bis zur Kreditentscheidung vergehen im Schnitt **ca. 5 Werktage**.

Folgen: Kunden wandern zu Direktbanken mit Sofortzusage ab, die Sachbearbeitung ist durch Routinefälle ausgelastet, und Medienbrüche führen zu Erfassungsfehlern.

## Ziele

| Ziel | Heute | Zielwert |
|---|---|---|
| Zeit bis zur (Vor-)Entscheidung | ca. 5 Werktage | **unter 10 Minuten** für Standardfälle |
| Abbruchquote im Antragsprozess | nicht gemessen | **unter 30 %**, je Schritt messbar |
| Manuell bearbeitete Anträge | 100 % | **max. 30 %** (nur Sonderfälle) |

## Stakeholder

| Stakeholder | Interesse | Rolle im Projekt |
|---|---|---|
| Privatkunde | Schnelle, einfache Antragstellung ohne Filialbesuch | Endnutzer, Input über Interviews und Journey |
| Kreditsachbearbeitung | Weniger Routinefälle, vollständige Antragsdaten | Fachexperte, Abnahme der Prozesse |
| Risikomanagement | Kreditrisiko kontrollieren, Entscheidungsregeln steuern | Liefert Scoring- und Entscheidungsregeln |
| Compliance / Datenschutz | Einhaltung von MaRisk, DSGVO und Verbraucherkreditrecht | Prüft Anforderungen, Freigabe |
| Product Owner (Privatkundengeschäft) | Marktanteil, Kundenzufriedenheit | Priorisiert das Backlog |
| IT / Entwicklungsteam | Klare, umsetzbare Anforderungen und Schnittstellen | Umsetzung, Schätzung der Stories |

## Scope

**Im Scope**
- Ratenkredite für Privatkunden bis 50.000 €
- Online-Antragsstrecke (Web, mobilfähig)
- Automatische Vorprüfung inkl. SCHUFA-Abfrage und Vorentscheidung
- Weiterleitung von Sonderfällen an die Sachbearbeitung

**Nicht im Scope**
- Baufinanzierung und Geschäftskundenkredite
- Auszahlung und Vertragsverwaltung nach Abschluss
- Änderungen am Kernbanksystem

## Vorgehen & Artefakte

| Artefakt | Inhalt | Datei |
|---|---|---|
| Prozessmodell (BPMN) | Ist- und Soll-Prozess mit markierten Schwachstellen | [diagramme/](diagramme/) |
| Customer Journey Map | Phasen, Touchpoints, Pain Points aus Kundensicht | [diagramme/](diagramme/) |
| Epics & User Stories | Anforderungen mit Akzeptanzkriterien (Given/When/Then) | [docs/](docs/) |
| KPI-Auswertung (SQL) | Kennzahlen auf Basis des öffentlichen German-Credit-Datensatzes | [sql/](sql/) |

Datenbasis: [Statlog (German Credit Data)](https://archive.ics.uci.edu/dataset/144/statlog+german+credit+data), UCI Machine Learning Repository – 1.000 anonymisierte Kreditanträge einer deutschen Bank.

## Nächste Schritte

- Schnittstelle zur SCHUFA als API-Spezifikation (OpenAPI) ausarbeiten
- Ablauf der Vorprüfung als UML-Sequenzdiagramm modellieren
- Entscheidungsregeln des Risikomanagements als Entscheidungstabelle (DMN) dokumentieren
- Klickbaren Prototyp der Antragsstrecke mit Nutzern testen
