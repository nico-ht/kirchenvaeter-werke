# Kirchenväter Werke

Deutsche Übersetzungen frühchristlicher Werke von [Die ersten Christen](https://www.erste-christen.de).
Lies mit, lade Texte herunter und hilf uns, Übersetzungen und Anmerkungen zu verbessern.

**Nicht kommerziell · Quelle nennen · Bearbeitungen unter gleicher Lizenz**

[Texte lesen](werke/) · [Archiv herunterladen](https://github.com/nico-ht/kirchenvaeter-werke/archive/refs/heads/main.zip) · [Mitmachen](CONTRIBUTING.md) · [Lizenz](LICENSE.md)

## Was du hier findest

Eigene deutsche Übersetzungen und öffentliche Anmerkungen von **Die ersten Christen**,
bereitgestellt unter [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.de), soweit Schutzrechte bestehen.
Die Lizenz betrifft unsere Beiträge, nicht gemeinfreie Ausgangswerke oder gesetzlich erlaubte Nutzungen.
Griechische, lateinische, englische und fremde deutsche Fassungen sind nicht Bestandteil dieses Archivs.

Die Texte sind nach **Autor → Werksammlung → Werk → Kapitel** geordnet.
Werke ohne Sammlung stehen direkt beim Autor. Die Verzeichnisse verwenden die vorhandenen Website-Titel.
In jedem Werk findest du ein Inhaltsverzeichnis; jedes Kapitel liegt als lesbares Markdown und als strukturiertes JSON vor.

| Datei | Inhalt |
| --- | --- |
| `werke/` | Werke und Kapitel mit öffentlichen Fußnoten und Quellenangaben |
| `catalogue.json` | Übersicht aller veröffentlichten Werke im Archiv |
| `paths.json` | Zuordnung stabiler Werk-IDs zu den aktuellen Verzeichnissen |
| `corrections/` | Eingereichte Korrekturvorschläge, sobald vorhanden |

Der Git-Verlauf macht veröffentlichte Änderungen nachvollziehbar. Eine nächtliche Codex-Automation gleicht die veröffentlichten Fassungen ab: ein Commit je geändertem Werk, getrennte Commits für Archivverzeichnisse und Dokumentation. Ohne Änderungen entstehen keine Commits.

## Änderungen lesen

Öffne im Commit die betroffene `kapitel-NNN.md`. Kurze Textzeilen an Satz- und Teilsatzgrenzen
machen Korrekturen sichtbar; GitHub kann innerhalb geänderter Zeilen einzelne Wörter hervorheben.
Beim Lesen bleiben die Absätze zusammenhängend. Technische JSON-Dateien sind im Diff standardmäßig
eingeklappt und können bei Bedarf geöffnet werden. Inhaltsrevisionen stehen weiterhin im JSON.

Lokal zeigt `git log -p --word-diff=color -- 'werke/**/*.md'` die Wortänderungen im Verlauf.
Für einen bestimmten Werk-Commit verwende `git show --word-diff=color COMMIT-ID -- 'werke/**/*.md'`.

## Lokal lesen und aktuell halten

Mit Git erhältst du das Archiv einschließlich seiner Versionsgeschichte:

```sh
git clone https://github.com/nico-ht/kirchenvaeter-werke.git
cd kirchenvaeter-werke
```

Später holst du neue Fassungen in diesem Verzeichnis mit:

```sh
git pull --ff-only
```

Das aktualisiert deine lokale Kopie. Ein **Pull Request** ist dagegen ein Vorschlag,
eine eigene Änderung in dieses Repository zu übernehmen. Die [Mitmach-Anleitung](CONTRIBUTING.md) erklärt den Ablauf.
Ohne Git kannst du das [gesamte Archiv als ZIP herunterladen](https://github.com/nico-ht/kirchenvaeter-werke/archive/refs/heads/main.zip).

## Hilf mit

Ein Tippfehler, eine unklare Übersetzung oder eine fragliche Anmerkung?
[Erstelle einen Fehlerhinweis](https://github.com/nico-ht/kirchenvaeter-werke/issues/new?template=fehlerhinweis.yml)
mit Werk, Kapitel und möglichst einem konkreten Vorschlag.
Du kannst auch einen [Pull Request vorbereiten](CONTRIBUTING.md#mit-github-einen-pull-request-einreichen).

Auf der [Website](https://www.erste-christen.de/werke) kannst du direkt beim Kapitel eine Änderung prüfen und als öffentlichen Pull Request einreichen – auch ohne GitHub-Konto.
Dein verifiziertes GitHub-Profil kannst du freiwillig angeben; den Pull Request erstellt unsere App.
Die Redaktion prüft den Vorschlag. Nach dem Zusammenführen erfolgt eine gesonderte Übernahme auf die Website.

## Quelle nennen

Bei einer Weiterverwendung unserer Übersetzungen oder Anmerkungen nennst du **Die ersten Christen**
mit einem Verweis auf **https://www.erste-christen.de**, der genauen Textstelle und der Lizenz. Zum Beispiel:

> Die ersten Christen: [Werk, Kapitel], deutsche Übersetzung. https://www.erste-christen.de · Textstelle: [Textstellen-URL].
> Lizenz: CC BY-NC-SA 4.0 (https://creativecommons.org/licenses/by-nc-sa/4.0/). Änderungen: [keine / Beschreibung].

Kommerzielle Nutzung ist durch diese Lizenz nicht erlaubt. Veröffentlichte Bearbeitungen unserer Beiträge
müssen unter derselben Lizenz stehen. Die vollständigen Bedingungen stehen in [LICENSE.md](LICENSE.md).
