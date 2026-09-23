# Kirchenväter Werke

Eigene deutsche Übersetzungen frühchristlicher Werke und öffentliche Fußnoten von
[Die ersten Christen](https://www.erste-christen.de).

**Nicht kommerziell · Quelle nennen und verlinken · Bearbeitungen unter gleicher Lizenz**

Unsere Beiträge stehen unter [CC BY-NC-SA 4.0](LICENSE.md), soweit Schutzrechte bestehen.
Gemeinfreie Ausgangswerke und gesetzlich erlaubte Nutzungen bleiben davon unberührt.

[Werke](werke/) · [Auf der Website lesen](https://www.erste-christen.de/werke) · [Archiv herunterladen](https://github.com/nico-ht/kirchenvaeter-werke/archive/refs/heads/main.zip)

## Aufbau

Autor → Werksammlung → Werk → Kapitel. Werke ohne Sammlung stehen direkt beim Autor.
Jedes Kapitel ist eine Markdown-Datei mit normalen Absätzen und Fußnoten, direkt auf GitHub lesbar
und als Text für eigene Werkzeuge und KI-Anwendungen nutzbar.
Unter `werke/` liegen ausschließlich Markdown-Dateien. Die kleine Datei `.sync/index.json`
ordnet Werk-IDs, Pfade und Prüfwerte für den automatischen Abgleich zu; sie enthält keine Texte.

## Mitmachen

Tippfehler, Übersetzungsfehler oder eine fragliche Anmerkung entdeckt?
[Erstelle einen Fehlerhinweis](https://github.com/nico-ht/kirchenvaeter-werke/issues/new?template=fehlerhinweis.yml)
oder folge der [Anleitung für Pull Requests](CONTRIBUTING.md).

Auf der [Website](https://www.erste-christen.de/werke) kannst du direkt beim Kapitel eine Korrektur
vorschlagen – auch ohne GitHub-Konto. Die Redaktion prüft und übernimmt Vorschläge.
Ein GitHub-Merge allein ändert den Website-Text noch nicht.

## Lokal nutzen

```sh
git clone https://github.com/nico-ht/kirchenvaeter-werke.git
cd kirchenvaeter-werke
git pull --ff-only
```

Der nächtliche Abgleich erzeugt einen Commit je geändertem Werk. Ohne Änderung entsteht kein Commit.
Im Commit zeigt `kapitel-NNN.md` den Textvergleich; GitHub kann geänderte Wörter hervorheben.
Die technische Zuordnung ist im Diff standardmäßig eingeklappt. Für einen lokalen Wortvergleich:

```sh
git show --word-diff=color COMMIT-ID -- 'werke/**/*.md'
```

## Quelle nennen

Bei Weiterverwendung: **Die ersten Christen**, Link zu **https://www.erste-christen.de** und zur
verwendeten Textstelle, **CC BY-NC-SA 4.0** mit [Lizenzlink](https://creativecommons.org/licenses/by-nc-sa/4.0/).
Änderungen bitte kennzeichnen. Kommerzielle Nutzung ist durch diese Lizenz nicht erlaubt;
veröffentlichte Bearbeitungen müssen unter derselben Lizenz stehen.
