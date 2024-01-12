# Projektname

Eine kurze Beschreibung Ihres Projekts. Dies sollte das Hauptziel und den Zweck Ihres Projekts klar umreißen.

## Einleitung

Geben Sie eine detailliertere Beschreibung Ihres Projekts. Erklären Sie, was dieses Projekt macht und warum es nützlich ist.

## Installation

Beschreiben Sie die Schritte zur Installation Ihres Projekts.

```bash
git clone https://github.com/ju1-eu/hello-world.git
cd hello-world
```

## Verwendung

Zeigen Sie, wie das Projekt verwendet wird. Erklären Sie die verschiedenen Funktionen und wie sie genutzt werden können.

```bash
# Entwickeln auf Feature-Branches
# Überprüfe den Status meiner Branches
git branch -a
git log --oneline --graph --all
# Neuen Branch und wechseln
git checkout -b dev
# Branch wechseln
git checkout dev
# Branch erstellen
git branch feature/new-feature-system
git branch bugfix/new-feature-systemn-error
git branch docs/update-readme
# Branch wechseln
git checkout docs/update-readme

# Änderungen hinzufügen und committen
vim README.md
git add .
git commit -m"update README - Verwendung"
git status
# Aktualisieren - Änderungen Pushen
git push origin docs/update-readme
git log --oneline --graph --all

# Einen Pull Request Erstellen, Mergen, Repository Aktualisieren, Aufräumen
# Pull Request erstellen
gh pr create --base main --title "Update README" --body "Meine ersten Änderungen - Hallo Welt"
# Pull Request nach Überprüfung mergen
# Code fehlerfrei? Teste Änderungen, bevor in den dev Branch mergen
gh pr merge docs/update-readme
    # ? What merge method would you like to use? Create a merge commit (=> Commits werden vom Branch in Hauptbranch gemergt.)
    # ? Delete the branch locally and on GitHub? No (=> nicht löschen)
    # ? What's next? Submit  (=> Bestätigen und den Merge-Prozess abschließen)
# Aktualisieren - Lokales Repository mit dem Hauptbranch synchronisieren
git checkout main
git pull origin main
git log --oneline --graph --all
# Aufräumen - Lokalen und Remote Branch löschen
git branch -d docs/update-readme
git push origin --delete docs/update-readme
git log --oneline --graph --all
```

## Mitwirken

Pull Requests sind willkommen. Für größere Änderungen öffnen Sie bitte zuerst ein Issue, um zu besprechen, was Sie ändern möchten.


## Lizenz

[MIT](https://choosealicense.com/licenses/mit/)


## Kontakt

Jan Unger – [Website](https://bw-ju.de/) – esel573@gmail.com

Projektlink: <https://github.com/ju1-eu/hello-world>


