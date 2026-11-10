# User Stories – Digitaler Ratenkredit

Abgeleitet aus den Pain Points der [Customer Journey](../diagramme/customer_journey.drawio).

| Epic | Stories |
|---|---|
| Online-Antragsstrecke | US-01, US-02, US-03 |
| Automatische Entscheidung & digitaler Abschluss | US-04, US-05, US-06 |

---

## US-01: Transparenter Kreditrechner

**Epic:** Online-Antragsstrecke · **Priorität:** Should · **Story Points:** 3

**User Story:**
Als Kundin möchte ich meine monatliche Rate und meine persönlichen Konditionen sehen, damit ich Angebote vergleichen kann, ohne meinen SCHUFA-Score zu verschlechtern.

**Akzeptanzkriterien:**
1. Gegeben ich bin auf der Website, wenn ich Betrag und Laufzeit eingebe, dann sehe ich sofort Monatsrate, effektiven Jahreszins und Gesamtkosten.
2. Gegeben ich möchte meine persönlichen Konditionen sehen, wenn ich die Konditionsanfrage absende, dann wird die SCHUFA-Anfrage SCHUFA-neutral gestellt.

---

## US-02: Checkliste vor dem Antrag

**Epic:** Online-Antragsstrecke · **Priorität:** Should · **Story Points:** 2

**User Story:**
Als Kundin möchte ich vor dem Start eine Checkliste der benötigten Unterlagen sehen, damit ich den Antrag ohne Unterbrechung ausfüllen kann.

**Akzeptanzkriterien:**
1. Gegeben ich starte den Antrag, wenn ich die erste Seite öffne, dann sehe ich eine Liste aller benötigten Unterlagen und Angaben.
2. Gegeben ich bin angestellt oder selbstständig, wenn ich meine Beschäftigungsart auswähle, dann passt sich die Checkliste an.

---

## US-03: Digitaler Kontoblick statt Upload

**Epic:** Online-Antragsstrecke · **Priorität:** Should · **Story Points:** 5

**User Story:**
Als Kundin möchte ich der Bank einen digitalen Kontoblick freigeben, damit ich keine Gehaltsnachweise hochladen muss.

**Akzeptanzkriterien:**
1. Gegeben ich bin im Antrag, wenn ich den Kontoblick freigebe, dann werden Einkommen und regelmäßige Ausgaben automatisch übernommen.
2. Gegeben ich möchte den Kontoblick nicht nutzen, wenn ich „Nachweise hochladen“ wähle, dann kann ich die Dokumente manuell hochladen.
3. Gegeben ich gebe den Kontoblick frei, wenn die Daten übernommen werden, dann wird meine Einwilligung DSGVO-konform gespeichert.

---

## US-04: Vorabzusage in unter 10 Minuten

**Epic:** Automatische Entscheidung & digitaler Abschluss · **Priorität:** Must · **Story Points:** 8

**User Story:**
Als Kundin möchte ich innerhalb weniger Minuten eine Vorabentscheidung erhalten, damit ich schnell weiß, ob ich den Kredit bekomme.

**Akzeptanzkriterien:**
1. Gegeben mein Antrag ist vollständig, wenn das Scoring „grün“ ergibt, dann erhalte ich innerhalb von 10 Minuten eine Vorabzusage.
2. Gegeben das Scoring ergibt „rot“, wenn die Entscheidung angezeigt wird, dann sehe ich eine verständliche Begründung der Ablehnung.
3. Gegeben das Scoring ergibt „gelb“, wenn die Entscheidung erfolgt, dann wird der Antrag an die Sachbearbeitung weitergeleitet und ich werde darüber informiert.

---

## US-05: Statusanzeige

**Epic:** Automatische Entscheidung & digitaler Abschluss · **Priorität:** Should · **Story Points:** 3

**User Story:**
Als Kundin möchte ich jederzeit den Status meines Antrags sehen, damit ich weiß, wie lange ich noch warten muss.

**Akzeptanzkriterien:**
1. Gegeben ich habe einen Antrag gestellt, wenn ich die Statusseite öffne, dann sehe ich den aktuellen Schritt (eingegangen, in Prüfung, entschieden).
2. Gegeben der Status ändert sich, wenn ein neuer Schritt erreicht ist, dann erhalte ich eine E-Mail oder Push-Nachricht.

---

## US-06: Mehrere Ident-Optionen

**Epic:** Automatische Entscheidung & digitaler Abschluss · **Priorität:** Must · **Story Points:** 5

**User Story:**
Als Kundin möchte ich zwischen mehreren Identifikationsverfahren wählen, damit ich den Vertrag auch dann abschließen kann, wenn ein Verfahren nicht funktioniert.

**Akzeptanzkriterien:**
1. Gegeben ich habe eine Vorabzusage, wenn ich zur Identifikation komme, dann kann ich zwischen Video-Ident und eID wählen.
2. Gegeben die Identifikation war erfolgreich, wenn ich den Vertrag digital unterschreibe, dann wird der Kredit am selben Werktag ausgezahlt.
