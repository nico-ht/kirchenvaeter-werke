# Mitmachen

Danke, dass du unsere Übersetzungen und öffentlichen Anmerkungen verbessern möchtest.
Schon ein genauer Hinweis mit Werk und Kapitel hilft.

## Einen Fehler melden

Öffne das [Formular für einen Fehlerhinweis](https://github.com/nico-ht/kirchenvaeter-werke/issues/new?template=fehlerhinweis.yml).
Nenne Autor, Werk und Kapitel, zitiere die betreffende Stelle und erkläre kurz, was dir aufgefallen ist.
Ein konkreter Ersatztext ist willkommen; bei einer Übersetzungsfrage hilft eine nachvollziehbare Quellenangabe.
Prüfe vorher die [offenen Hinweise](https://github.com/nico-ht/kirchenvaeter-werke/issues), damit wir dieselbe Stelle gemeinsam besprechen können.

Hinweise, Pull Requests und darin genannte Namen sind öffentlich. Bitte veröffentliche keine persönlichen Kontaktdaten.
Übernimm keine geschützten fremden Übersetzungen ohne passende Erlaubnis.

## Über die Website vorschlagen

Auf der Website kannst du Vorschläge ohne GitHub-Konto einreichen:

1. Öffne das betreffende Kapitel unter [Werke](https://www.erste-christen.de/werke), markiere die Textstelle und wähle **„Änderung vorschlagen“**. Alternativ findest du die Aktion am Kapitelende.
2. Gib die kurze, eindeutige Textstelle, deinen Ersatztext und eine Begründung an. Ein öffentlicher Anzeigename ist freiwillig.
3. Prüfe die Vorschau und bestätige die Beitragslizenz **CC BY-NC-SA 4.0**.
4. Reiche den Vorschlag ein. Unsere App erstellt den öffentlichen Pull Request für dich; du brauchst dafür kein GitHub-Konto. Dein verifiziertes GitHub-Profil kannst du freiwillig beim Vorschlag angeben.

Eine Vorschau oder ein Download allein reicht noch keinen Vorschlag ein.
Wenn der direkte Versand nicht verfügbar ist, kannst du die geprüfte Vorschlagsdatei herunterladen und selbst auf GitHub einreichen.

## Werke und Autoren vorschlagen

In der [Werkübersicht](https://www.erste-christen.de/werke#werk-wunsch) kannst du über **„Werkwunsch senden“** ein Werk oder einen Autor wünschen.
Gib Autor und Wunsch an; bei einem Werkwunsch zusätzlich den Titel. Ein Quellenlink und die Quellsprache
(Griechisch, Latein, Syrisch oder Englisch) sind freiwillig. Eine geeignete Quelle kann später recherchiert werden.
Prüfe die Vorschau und stimme der öffentlichen Veröffentlichung deines eigenen Beitrags unter CC BY-NC-SA 4.0 zu.
Die App erstellt einen Pull Request mit einer Datei `work-requests/<preview-hash>.json`.
Alternativ kannst du die Vorschlagsdatei herunterladen und unter diesem Pfad in deinem Fork einreichen.

Der Pull Request enthält einen kopierbaren Codex-Auftrag zur Quellenprüfung und Vorbereitung des MCP-Imports.
Die Redaktion prüft Dubletten, Autorenzuordnung und Quellenrechte. Fehlende Autoren oder Quellen werden zuerst geklärt.
Import und Übersetzung starten erst nach ausdrücklichem Auftrag der Redaktion in Codex über den freigegebenen
ChurchFathers-MCP-Workflow. Ein Wunsch oder Merge allein startet keine Übersetzung.

## Mit GitHub einen Pull Request einreichen

Für eine Textkorrektur wird eine von der Website erzeugte Vorschlagsdatei benötigt.
Das erhält den Bezug zur geprüften Ausgangsfassung und ermöglicht die spätere redaktionelle Übernahme.
So bereitest du einen eigenen Pull Request vor:

1. Erzeuge dort die Vorschau, stimme der Beitragslizenz zu und wähle **„Vorschlag für Pull Request herunterladen“**.
   Die Datei heißt `<preview-hash>.json`; lass ihren Namen und Inhalt unverändert.
2. [Erstelle einen Fork](https://github.com/nico-ht/kirchenvaeter-werke/fork) dieses Repositories in deinem GitHub-Konto.
3. Erstelle in deinem Fork einen neuen Branch, zum Beispiel `korrektur/werk-kapitel`.
4. Lege die heruntergeladene Datei im Ordner `corrections/` ab. Das geht lokal mit Git oder auf GitHub über **Add file → Upload files**.
   Falls der Ordner noch fehlt, kannst du über **Add file → Create new file** den Pfad `corrections/<preview-hash>.json` anlegen und den vollständigen Dateiinhalt einfügen.
5. Committe nur diese eine Vorschlagsdatei. Öffne über **Contribute → Open pull request** einen Pull Request
   gegen **`nico-ht/kirchenvaeter-werke`**, Zielbranch **`main`**. Nenne Werk, Kapitel und den Grund für die Änderung.

Pro Pull Request ist genau **eine** Datei `corrections/<preview-hash>.json` vorgesehen.
Erzeuge für weitere Korrekturen jeweils einen eigenen Vorschlag und Branch.
Wenn du den Ersatztext nachträglich ändern möchtest, erstelle eine neue Vorschau auf der Website und lade die neue Datei herunter.

### Optional: mit Git arbeiten

Klone über **Code** die URL deines eigenen Forks. Im lokalen Klon legst du dann den Branch an:

```sh
git switch -c korrektur/werk-kapitel
mkdir -p corrections
```

Kopiere die heruntergeladene Datei nach `corrections/`. Ersetze im folgenden Befehl den Platzhalter durch ihren tatsächlichen Namen:

```sh
git add corrections/DEIN-DATEINAME.json
git commit -m "fix(text): propose chapter correction"
git push -u origin korrektur/werk-kapitel
```

Öffne anschließend den von GitHub angebotenen Pull-Request-Link und prüfe das Zielrepository und den Zielbranch.
Zum reinen Lesen und Aktualisieren des offiziellen Archivs stehen die Befehle in der [README](README.md#lokal-lesen-und-aktuell-halten).

## Was danach passiert

Die Redaktion prüft den Vorschlag und kann Rückfragen im Pull Request stellen.
Ein zusammengeführter Pull Request ändert noch keinen Website-Text: Die Redaktion prüft die identische Vorschau
zusätzlich im Website-Backend und übernimmt sie dort ausdrücklich. Passt die Ausgangsfassung inzwischen nicht mehr,
ist eine neue Vorschau erforderlich. Bei erfolgreicher Übernahme bestätigt ein Kommentar den Website-Stand;
das Archiv folgt beim nächsten Abgleich.

Die Dateien unter `werke/`, die Verzeichnisse und diese Dokumentation werden aus der Website-Anwendung erzeugt.
Direkte Änderungen daran können beim Abgleich überschrieben werden. Nutze für Textkorrekturen den beschriebenen Vorschlagsweg;
Ideen zur Navigation, Dokumentation oder zu weiteren eigenen Übersetzungen kannst du als
[Issue](https://github.com/nico-ht/kirchenvaeter-werke/issues/new) besprechen.

Mit der Einreichung eines eigenen Textbeitrags bestätigst du, dass er unter **CC BY-NC-SA 4.0** veröffentlicht werden darf.
Für die Weiterverwendung gelten **nicht kommerziell, Quelle nennen, Bearbeitungen unter gleicher Lizenz**;
Näheres steht in [LICENSE.md](LICENSE.md).
