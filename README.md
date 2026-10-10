# lernspiele
Interaktive Lernspiele für den Mathematikunterricht – direkt im Browser, ohne Anmeldung.

## Spiele

| Spiel | Unterrichtsdatum | Schülerlink |
|---|---|---|
| Drei Verfahren (quadratische Gleichungen: Wurzelziehen, Ausklammern, pq-Formel) | 12.10.2026 | https://tonchime.github.io/lernspiele/ |
| Drei Verfahren, ChatGPT-Version (wird nur von ChatGPT bearbeitet) | 12.10.2026 | https://tonchime.github.io/lernspiele/chatgpt/ |

Jedes Spiel hat drei Stufen: Paare zuordnen, Lückentext mit Auswahl aus Liste, Lückentext zum Einschreiben.

## Ablage
- Das Spiel im Hauptverzeichnis (`index.html`) ist das Startspiel unter der Hauptadresse.
- Zwei getrennte Fassungen: `index.html` im Hauptverzeichnis ist die Claude-Version (im Spiel oben als „Claude-Version“ gekennzeichnet); `chatgpt/index.html` ist die ChatGPT-Version und wird ausschließlich von ChatGPT bearbeitet. Keine Fassung überschreibt die andere.
- Jedes weitere Spiel bekommt einen eigenen Unterordner unter `spiele/`, zum Beispiel `spiele/2026-10-16-wiederholung/index.html`, und einen eigenen Schülerlink `https://tonchime.github.io/lernspiele/spiele/2026-10-16-wiederholung/`.
- Ein überarbeitetes Spiel bleibt in seinem bisherigen Ordner, damit der Link gleich bleibt.

## Neues Spiel anlegen
Alle Spiele entstehen aus der Vorlage `vorlage/index.html` (Grundlage: Claude-Version v7). Spielablauf und Gestaltung sind darin festgelegt; geändert wird nur der Inhaltsblock am Anfang der Datei.

1. Ordner `spiele/<datum>-<thema>/` anlegen, z. B. `spiele/2026-10-16-wiederholung/` (Kleinbuchstaben, Bindestriche, keine Umlaute).
2. `vorlage/index.html` als `index.html` in diesen Ordner kopieren.
3. Nur den Block zwischen „INHALT DES SPIELS“ und „ENDE DES INHALTSBLOCKS“ füllen: Titel, Datum, Versionsmarke, Paare für Stufe 1 (höchstens 6), Auswahlzeilen für Stufe 2 (richtige Möglichkeit mit `*`), Gleichungen mit Lösungen für Stufe 3, Hilfetexte.
4. Schülerlink: `https://tonchime.github.io/lernspiele/spiele/<datum>-<thema>/`. Spiel oben in der Tabelle eintragen.

Die Vorlage selbst ist unter `https://tonchime.github.io/lernspiele/vorlage/` mit dem Inhalt vom 12.10.2026 spielbar.

## Vorlage auch für die ChatGPT-Version
Auch die ChatGPT-Version baut neue Spiele aus `vorlage/index.html`, damit alle Spiele gleich funktionieren und aussehen.

- ChatGPT legt seine Spiele unter `chatgpt/spiele/<datum>-<thema>/index.html` ab, z. B. `chatgpt/spiele/2026-10-16-wiederholung/`. Schülerlink: `https://tonchime.github.io/lernspiele/chatgpt/spiele/<datum>-<thema>/`.
- Geändert wird auch dort nur der Block zwischen „INHALT DES SPIELS“ und „ENDE DES INHALTSBLOCKS“; als Versionsmarke „ChatGPT-Version · v1“, bei jeder Überarbeitung eine Zahl höher.
- `vorlage/`, die `index.html` im Hauptverzeichnis und `spiele/` werden von Claude gepflegt; `chatgpt/` wird ausschließlich von ChatGPT gepflegt. Keine Seite verändert die Dateien der anderen. Änderungswünsche an der Vorlage gehen als Vorschlag an Tony.
- Vor jedem Upload den aktuellen Stand von `main` lesen, nur eigene Dateien ändern, nie force-pushen, keine fremden Dateien löschen oder überschreiben.
- Jedes neue Spiel wird mit Titel, Unterrichtsdatum und Schülerlink in die Tabelle oben eingetragen.
