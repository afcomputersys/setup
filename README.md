# setup
Informationen zur Einrichtung von Git und GitHub

## Installation
`git` kann via Xcode-Befehlszeilentools installiert werden.

Dazu einfach im Terminal folgendes eingeben:

```shell
admin@mac ~ $ xcode-select --install
```

Und die Installation im Dialogfenster bestätigen.

Anschliessend Benutzername und Mailadresse in der Konfiguration eintragen:

```shell
admin@mac ~ $ git config --global user.name "Philipp Ming"
admin@mac ~ $ git config --global user.email "pming@a-f.ch"
```

Die GitHub-App kann [hier](https://desktop.github.com) heruntergeladen werden.

## Anwendung
Git / GitHub wird hauptsächlich für die Versionsverwaltung bei der Programmierung verwendet, kann aber für vieles mehr nützlich sein; beispielsweise für die Versionsverwaltung von Scripts.

### Repositories
Pro "Projekt" soll ein separates Repository verwendet werden. Mit einem Gratiskonto können unbegrenzt öffentliche Repositories angelegt werden.
Links zu Repositories auf GitHub sind wie folgt aufgebaut:

* github.com/organisation/repository
* github.com/benutzer/repository
* github.com/munki/munki

Ein neues Repository kann via Browser auf GitHub, via GitHub-App oder via Befehlszeile erstellt werden. Im Dateisystem entspricht ein Repository einem Verzeichnis.

Mittels Befehlszeile kann ein Repository wie folgt angelegt werden:

```shell
admin@mac ~ $ cd Projekte
admin@mac ~/Projekte $ git init supersoftware
```

Das Repository wird lokal gelöscht, indem das Verzeichnis gelöscht wird.
Um das Repository auf GitHub zu löschen, muss man es direkt auf GitHub löschen.

In den Einstellungen des jeweiligen Repository können die Berechtigungen von einzelnen Personen oder einem ganzen Team angepasst werden.

### Grundlagen von Git
Der grundlegende Ablauf für die Verwendung von Git sieht wie folgt aus:

1. Letzte Änderungen vom Git-Server (GitHub) kopieren (git pull)
2. Anpassungen an den Dateien vornehmen
3. Programm / Script testen, etc.
4. Dateien für Commit hinzufügen (git add)
5. "Committen" (git commit)
6. Änderungen auf Git-Server (GitHub) kopieren (git push)

Der ganze Ablauf kann für vereinfacht mit der GitHub-App durchgearbeitet werden.

1. "Fetch Origin" in der GitHub-App klicken, um neuste Änderungen zu erhalten. Wenn es Neuigkeiten gibt, erneut mit "Pull Origin" bestätigen, um die Änderungen zu übernehmen.
2. Anpassungen an Scripts, Dateien, etc. vornehmen
3. Scripts testen
4. Die GitHub-App fügt geänderte Dateien automatisch hinzu
5. Die geänderten Dateien, die man definitiv hinzufügen möchte, kann man wählen. Dazu soll in jedem Fall eine "Commit-Message", in der beschrieben wird, was geändert wurde, hinzugefügt werden. Bei kleinen Commits reicht es, das "Summary"-Feld auszufüllen und anschliessend mit "Commit to master" zu bestätigen. Wenn grössere Änderungen vorgenommen werden, sollten diese ausführlich beschrieben werden. Es macht Sinn, zusammenhängende Änderungen in einem Commit abzusenden. Änderungen ohne Zusammenhang sollten in separate Commits gefasst werden.
6. Wenn man die Dateien im Repository auf dem lokalen Rechner änderte, müssen diese noch auf GitHub kopiert werden. Dies kann man mit dem Button "Push origin" vornehmen.

#### Branches
Bei grösseren Projekten kann man sogenannte Branches anlegen, was einem Zweig der "Hauptentwicklung" entspricht. Möchte man beispielsweise einzelne Features hinzufügen oder einzelne Fehler beheben, dann kann dafür ein Branch erzeugt werden, in dem es nur um das jeweilige sekundäre Ziel geht. Wenn der Fehler behoben oder das Feature im Branch hinzugefügt wurde, kann dieser wieder mit dem "Master" zusammengeführt werden.
Um beispielsweise einen Bugfix-Branch mit dem Master zusammenzuführen, muss ein Pull Request erstellt werden.

### Dokumentieren auf GitHub
Für die Dokumentation von Projekten verwendet GitHub die "Markdown"-Syntax.
[Hier](http://texwelt.de/wissen/markdown_help/) gibt's eine gekürzte Übersicht über Markdown.

## Zusätzliche Funktionen von GitHub
GitHub bietet zusätzlich die Möglichkeit "Issues" zu erstellen, in denen Anwender oder die Entwickler des Programms Pendenzen oder Probleme notieren und verfolgen können.

## Weiterführende Infos
Hier noch ein paar Links zu weiteren Guides, Tutorials, Referenzen, etc.:
r

* [GitHub Guides](https://guides.github.com)
* [Interaktives Tutorial zu Git](https://try.github.io/levels/1/challenges/1)
* [Übersicht über die wichtigsten Befehle](https://rogerdudler.github.io/git-guide/index.de.html)
* [Git-Tower (Alternative zu GitHub-App)](https://www.git-tower.com/mac/)
* [Übersicht mit Links zu Git](https://stefanimhoff.de/2009/einstieg-in-git-als-versionskontrollsystem/)
* [Detailliertes GitHub-Cheatsheet](https://github.com/tiimgreen/github-cheat-sheet)

## Text-Editoren mit eingebauter Git-Unterstützung

* [BBEdit](http://www.barebones.com/products/bbedit/)
* [TextMate](http://macromates.com)
* [Atom](https://atom.io)
* [Microsoft Visual Studio Code](https://code.visualstudio.com)
* [Adobe Brackets](http://brackets.io)

## Interessante Links auf GitHub für CLI-Programme, Shell-Scripting, etc.

* [Awesome Shell](https://github.com/alebcay/awesome-shell)
* [Python MacAdmin Tools](https://github.com/timsutton/python-macadmin-tools)
* [Scripts von Rich Trouton aka derflounder](https://github.com/rtrouton/rtrouton_scripts/tree/master/rtrouton_scripts)
* [Awesome command line apps](https://github.com/herrbischoff/awesome-command-line-apps)
* [Awesome OS X command line](https://github.com/herrbischoff/awesome-osx-command-line)
* [Sammlung erweiterbarer Script-Grundlagen](https://github.com/jmcantrell/bashful)
* [Awesome Sysadmin](https://github.com/n1trux/awesome-sysadmin)
* [Awesome GitHub (noch mehr Infos zu GitHub)](https://github.com/phillipadsmith/awesome-github)
