# openFriedhof

**Freie Software für die Friedhofsverwaltung von Kommunen und Kirchengemeinden.**

openFriedhof ist eine webbasierte, quelloffene Friedhofsverwaltung für den deutschen Rechtsrahmen. Jeder Friedhofsträger soll sie kostenlos nutzen, prüfen und weiterentwickeln können: Gemeinden und Ämter, evangelische und katholische Kirchengemeinden, Friedhofsvereine und ehrenamtliche Verwalterinnen und Verwalter.

> **Status:** Konzeptphase (November 2026). Es gibt noch keinen lauffähigen Code. Von Dezember 2026 bis Februar 2027 sprechen wir mit Friedhofsträgern in Vorpommern, um Pilotpartner zu gewinnen und das Datenmodell abzustimmen.

## Warum

- In Deutschland gibt es rund 32.000 Friedhöfe. Alle verwalten im Kern dasselbe: Grabstätten, Nutzungsrechte, Ruhefristen, Bestattungen, Gebühren und den Lageplan.
- Der Softwaremarkt dafür ist klein und vollständig proprietär. Die Daten liegen in geschlossenen Formaten, ein Wechsel ist aufwendig.
- Für den deutschen Rechtsrahmen gibt es bisher keine quelloffene Alternative.

openFriedhof soll eine gemeinsame, freie Grundlage schaffen. Die Daten bleiben beim Träger und sind jederzeit vollständig exportierbar.

## Grundsätze

- **Frei:** Lizenz EUPL 1.2, Veröffentlichung auf GitHub und openCode.
- **Offen in den Daten:** dokumentiertes Austauschformat, Import-Werkzeuge für bestehende Programme.
- **Für den deutschen Rechtsrahmen gebaut:** Ruhefristen, Nutzungszeiten und Gebühren werden nach der jeweiligen Friedhofs- und Gebührensatzung konfiguriert, nicht fest programmiert.
- **Einfach:** ohne Schulung nutzbar, auch für ehrenamtliche Verwalter.

## Geplanter Funktionsumfang

**Version 1.0**

- Grabkartei mit Grabarten, Lage, Belegung, Historie, Fotos und Dokumenten
- Nutzungsberechtigte, Nutzungsrechte mit Laufzeiten, Ruhefristen, Verlängerung und Übertragung; automatische Fristüberwachung
- Bestattungsvorgang als geführter Ablauf, Bestattungskalender
- Gebührenkatalog je Friedhof und Grabart, Bescheide und Rechnungen als PDF, Serienbriefe
- Lageplan mit Import vorhandener Pläne (Shape, GeoJSON), Grabflächen automatisch aus der Grabart
- Offlinefähige Web-App für den Außendienst: Grabzustand, Fotos, Standsicherheitsprüfung der Grabmale
- Datenübernahme aus Excel/CSV und aus Exporten verbreiteter Altprogramme

**Version 2.0**

- Öffentliche Grab- und Verstorbenensuche
- Terminanfrage und -anmeldung für Bestatter
- Empfang von Online-Anträgen (Bestattungsanmeldung, Erwerb von Grabnutzungsrechten) über FIT-Connect
- Integrierte Gebührenkalkulation

## Technik (geplant)

PHP mit Laravel, PostgreSQL mit PostGIS, MapLibre GL für Karten, Progressive Web App für den Außendienst, REST-API mit OpenAPI-Beschreibung, Betrieb per Docker Compose.

## Roadmap

| Phase | Zeitraum | Inhalt | Meilenstein |
|---|---|---|---|
| 0 | 12/2026 – 02/2027 | Gespräche mit Friedhofsträgern, Datenmodell | 1–2 Pilotpartner |
| 1 | 03/2027 – 08/2027 | Kernverwaltung | MVP im Parallelbetrieb beim Pilotpartner |
| 2 | 09/2027 – 02/2028 | Lageplan, Außendienst-App, Datenübernahme | Version 1.0 |
| 3 | 03/2028 – 12/2028 | Online-Dienste | Version 2.0 |
| 4 | ab 2029 | Partner, Community, Erweiterungen | |

Ausführlich: [Projektvorstellung](docs/openfriedhof-projektvorstellung.pdf) · [Marktanalyse](docs/openfriedhof-marktanalyse.pdf)

## Mitmachen

- **Friedhofsträger:** Als Pilotpartner gestalten Sie die Software mit und nutzen sie in der Pilotphase kostenlos, einschließlich Einrichtung.
- **Entwicklerinnen und Entwickler:** Siehe [CONTRIBUTING.md](CONTRIBUTING.md).
- **Förderer und Partner:** Unterstützung bei Finanzierung, Betrieb oder Verbreitung.

Kontakt: Andreas Hinderberger · andy@gertex.us

## Lizenz

openFriedhof steht unter der [Europäischen Open-Source-Lizenz EUPL 1.2](LICENSE).
