# Stamm Farm Auto

Ein Browser-Script für **Die Stämme**, das die täglichen Farm- und Sammeldaten eines Stammes ausliest, lokal speichert und automatisch einen fertigen Forumsbeitrag in BB-Code erstellt.

## Funktionen

- Liest Spielername, Stammesrang, Punkte, globalen Rang und Dörfer aus der Mitgliederübersicht.
- Ruft für alle Mitglieder die täglichen Werte **Geplündert** und **Gesammelt** ab.
- Berechnet automatisch den Gesamtwert.
- Speichert Tagesstände getrennt nach Welt und Stamm im Browser.
- Vergleicht den aktuellen Stand mit dem zuletzt gespeicherten älteren Tagesstand.
- Erstellt:
  - Top 5 nach Gesamtleistung
  - Top 5 nach höchster Steigerung
  - Durchschnittswerte
  - automatisches Fazit
  - vollständige farbige Rangliste mit `[player]`-Tags
- Kopiert den fertigen BB-Code und öffnet optional den gewünschten Forumslink.
- Veröffentlicht niemals selbstständig einen Beitrag.

## Installation

### TempMonk

1. Die Datei [`Stamm-Farm-Auto.txt`](Stamm-Farm-Auto.txt) öffnen.
2. Den vollständigen Inhalt kopieren.
3. In TempMonk ein neues Script anlegen.
4. Den Code einfügen und speichern.
5. Das Script in Die Stämme starten.

### Schnellleiste

1. Den vollständigen Inhalt von [`Stamm-Farm-Auto.txt`](Stamm-Farm-Auto.txt) kopieren.
2. In Die Stämme unter **Einstellungen → Schnellleiste** einen neuen Eintrag anlegen.
3. Den Code als Ziel einfügen und speichern.

## Bedienung

1. Das Script starten. Bei Bedarf wechselt es automatisch zur Stammes-Mitgliederübersicht.
2. Optional den Link zum Stammesforum oder gewünschten Thread eintragen.
3. **Daten lesen & Auswertung erstellen** anklicken.
4. Nach Abschluss den BB-Code kopieren oder über **Forum öffnen** zum gespeicherten Link wechseln.
5. Den Beitrag im Forum kontrollieren und manuell absenden.

Beim ersten gespeicherten Tag ist noch kein Vergleich möglich. Ab dem nächsten Tagesstand verwendet das Script automatisch den zuletzt gespeicherten älteren Stand.

## Datenspeicherung

Die Tagesstände und der optionale Forumslink werden ausschließlich im `localStorage` des verwendeten Browsers gespeichert. Es werden keine Zugangsdaten gespeichert und keine Daten an externe Dienste gesendet.

Die Historie umfasst maximal 120 Tagesstände je Welt und Stamm. Über **Rohdaten sichern** kann der aktuelle Stand zusätzlich als JSON-Datei heruntergeladen werden.

## Voraussetzungen

- Aktuelle deutsche Die-Stämme-Spielwelt
- Mitgliedschaft in einem Stamm
- Berechtigung, die Mitgliederübersicht aufzurufen
- Browser mit aktiviertem JavaScript

## Version

Aktuell: **1.0.0**

Details stehen in der [`CHANGELOG.md`](CHANGELOG.md).

## Hinweis

Das Script ist ein privates Hilfsmittel und kein offizielles Produkt von InnoGames. Vor einer breiteren Nutzung sollten die geltenden Spielregeln und Scriptbestimmungen der jeweiligen Welt geprüft werden.
