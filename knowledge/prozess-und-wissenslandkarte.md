## 1. Zweck und Abgrenzung
Diese Datei beschreibt den heutigen manuellen Ablauf, seine Entscheidungen, Regeln, Quellen, Ausnahmen, Risiken und offenen Fragen.
Sie enthält noch keine Skill-Implementierung.

## 2. Ausgangspunkt
- Referenzfall: `cases/F01-Raumbuchung.md`
- bisherige Antwort: `cases/F01-Emailantwort.md`
- die Antwort ist keine verbindliche Regelquelle

## 3. Beteiligte Rollen
| Rolle | Aufgabe |
|---|---|
| IT Support | Fall aufnehmen, Angaben prüfen, Entwurf vorbereiten |
| Controlling | Regeln und zulässige Zusagen bestätigen |
| Freigebende Rolle | Antwort vor externer Nutzung kontrollieren |
4.4 Eingaben und Normalablauf eintragen
## 4. Benötigte Eingaben
Pflicht: Zeitangabe, betroffen System, Fehlerbeschreibung, Fehlersituation und Kundenwunsch.
Optional: Tests, Nachweise, Screenshot, frühere Kommunikation und frühere Zusagen.
Fehlende entscheidungsrelevante Angaben werden erfragt und nicht ergänzt.

## 5. Manueller Normalablauf
| Nr. | Schritt | Ergebnis | Rolle |
|---:|---|---|---|
| 1 | Eingang lesen und Vorgang erfassen | Reklamationsfall | IT Support |
| 2 | Fehler dem System zuordnen | eindeutig oder Rückfrage | IT Support  |
| 3 | Mindestangaben prüfen | vollständig oder Rückfrage | IT Support  |
| 4 | Regeln und Quellen prüfen | belegte Aussagen oder Lücke | IT Support  |
| 5 | zulässige Lösung einordnen | Entwurfsgrundlage | IT Support  |
| 6 | Antwortentwurf und interne Prüfung trennen | interner Entwurf | IT Support  |
| 6 | finanzielle Entscheidung | interner Entwurf | Controlling  |
| 7 | Entwurf menschlich freigeben | freigegeben oder zurückgegeben | Freigebende Rolle |
4.5 Entscheidungspunkte eintragen
## 6. Entscheidungspunkte
### E01: Ist der Vorgang eindeutig zuordenbar?
- Ja: Mindestangaben prüfen.
- Nein: Referenz erfragen.
- Unklar: keine Entscheidung; gezielt nachfragen.

### E02: Sind die Mindestangaben vollständig?
- Ja: Risikoprüfung starten.
- Nein oder unklar: fehlende Angaben benennen.

### E03: Ist eine frühere Zusage belegt und berechtigt?
- Ja: Gültigkeit prüfen.
- Nein oder unklar: nicht übernehmen; Nachweis oder Entscheidung anfordern.

### E04: Erlaubt eine gültige Regel die gewünschte Lösung?
- Ja: im Entwurf berücksichtigen.
- Nein: nur belegte Alternative formulieren.
- Unklar: keine Zusage; an fachlichen Owner eskalieren.

### E05: Beträgt der finanzielle Aufwand mindestens 200 Euro?
- Ja: keine Zusage oder Beauftragung; Genehmigung durch Controlling anfordern.
- Nein: im normalen Prüfpfad fortfahren.
- Betrag unbekannt oder unklar: Betrag erfragen und keine finanzielle Zusage machen.
4.6 Wissensarten und Regelkarten eintragen
## 7. Wissensarten
- Fallfakt: gilt nur für den aktuellen Vorgang.
- Fachregel: steuert zulässiges Verhalten und benötigt Freigabe.
- Raumwissen: benötigt eine passende Quelle zur Beschreibung und Nutzung des Raums.
- Prozesswissen: beschreibt Rollen und Übergaben.
- Erfahrungswissen: bleibt Hinweis, bis es bestätigt wurde.

## 8. Regelkarten
### R01 Fehlende Angaben
- Aussage: Fehlende entscheidungsrelevante Angaben werden als Rückfrage ausgegeben.
- Quelle: Prozessbeschreibung des IT Support
- Owner: Controlling
- Status: zu bestätigen

### R02 Verbindliche Zusagen
- Aussage: Eine Zusage benötigt gültige Quelle und berechtigte Rolle.
- Quelle: fehlt
- Owner: Controlling
- Status: Wissenslücke

### R03 Genehmigung finanzieller Aufwände
- Aussage: Ab einem finanziellen Aufwand von 200 Euro ist vor einer Zusage oder Beauftragung die Genehmigung durch das Controlling erforderlich.
- Schwellenlogik: Kosten größer oder gleich 200 Euro.
- Genehmigende Rolle: Controlling
- Quelle: Festlegung für diesen Prozess
- Owner: Controlling
- Status: bestätigt


4.7 Quellen, Ausnahmen und Kontrollpunkte eintragen
## 9. Quellenlandkarte
| Quelle | Zweck | Status | Owner |
|---|---|---|---|
| `cases/F01-Raumbuchung.md` | Fallfakten | vorhanden | Workshop |
| `cases/F01-Emailantwort.md` | bisheriges Ergebnis | vorhanden, nicht verbindlich | Workshop |
| Lösungsrichtlinie | Zusagen | fehlt | Serviceleitung |
| Raumnutzung | Raumwissen | fehlt | Controlling |
| Regelkarte R03 in diesem Dokument | Genehmigung finanzieller Aufwände | bestätigt | Controlling |


## 10. Ausnahmen und Eskalationen
- fehlende Identifikation: Rückfrage an IT Support
- unbelegte Zusage: Controlling entscheidet
- widersprüchliche Quellen: getrennt dokumentieren; Owner klärt
- keine gültige Regel: keine Zusage; fachlich eskalieren

## 11. Menschliche Kontrollpunkte
- K01 Risikoprüfung vor einer Lösung
- K02 Quellen- und Zusagenprüfung vor verbindlicher Aussage
- K03 Freigabe vor externer Kommunikation
Der Skill darf keinen Kontrollpunkt selbst als bestanden markieren.
4.8 Qualität, Risiken und offene Fragen eintragen
## 12. Qualitätskriterien
- Jede verbindliche Aussage besitzt eine gültige Quelle.
- Fakten und Annahmen bleiben getrennt.
- Fehlende Angaben erscheinen als Rückfrage.
- Widersprüche bleiben sichtbar.
- Kundentext und interne Prüfung bleiben getrennt.
- Ergebnis bleibt als Entwurf markiert.
- finanzielle Entscheidung nur durch Controlling
- Bei Kosten ab 200 Euro liegt vor einer Zusage oder Beauftragung eine Genehmigung des Controllings vor.

## 13. Risiken
- erfundene Fakten: Rückfragen statt Ergänzung
- unbelegte Zusage: Quellenprüfung und Freigabe
- interne Information im Kundentext: getrennte Ausgabe


## 14. Offene Wissensfragen
- Ist eine Freigabe bei finanziellen Aufwand durch IT Support möglich  ?
- Welche internen Angaben dürfen nie in den Kundentext?

## 15. Übergang zu Modul 3
Bestätigte Aussagen werden in den Skill-Steckbrief übernommen. Offene Aussagen bleiben Lücke oder Eskalation.
