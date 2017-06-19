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

Die GitHub-App kann [hier](https://desktop.github.com) heruntergeladen werden, wird aber nicht zwingend benötigt.


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

### Grundlagen von Git
Der grundlegende Ablauf für die Verwendung von Git sieht wie folgt aus:

1. Letzte Änderungen vom Git-Server (GitHub) kopieren (git pull)
2. Anpassungen an den Dateien vornehmen
3. Programm / Script testen, etc.
4. Dateien für Commit hinzufügen (git add)
5. "Committen" (git commit)
6. Änderungen auf Git-Server (GitHub) kopieren (git push)

### Dokumentieren auf GitHub
Für die Dokumentation von Projekten verwendet GitHub die "Markdown"-Syntax.
[Hier](http://texwelt.de/wissen/markdown_help/) gibt's eine gekürzte Übersicht über Markdown.
