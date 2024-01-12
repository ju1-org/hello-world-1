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
# Dokumentationsupdates auf docs/update-readme
# Erstellen eines Branches für Dokumentationsupdates:
git branch -a
git log --oneline --graph --all
git checkout dev
git checkout -b docs/update-readme

# Durchführen von Änderungen an der Dokumentation:
vim README.md
vim .gitignore
git add .
git commit -m "Update README und .gitignore mit neuen Informationen"
git status

# Pushen des Dokumentationsbranches:
git push --set-upstream origin docs/update-readme

# Erstellen eines Pull Requests von `dev` nach `main`
# Mergen des Dokumentationsbranches in `dev`:
git checkout dev
git pull origin main
git merge docs/update-readme
git push origin dev

# Erstellen des Pull Requests von `dev` nach `main`:
gh pr create --base main --head dev --title "Aktualisierung der Dokumentation" --body "Fügt detaillierte Informationen zur README hinzu."

# Merge des Pull Requests:
# Liste aller offenen Pull Requests anzeigen [PR-Nummer]
gh pr list
gh pr view 2
#gh pr view 2 --web
# Code-Review durchführen
# Genehmigen eines Pull Requests
gh pr review 2 --approve
# PR ablehnen
#gh pr review 2 --request-changes "Bitte Code überprüfen"
gh pr merge 2
gh pr view 2
# Löschen des Feature-Branches:
git branch -d docs/update-readme
git push origin --delete docs/update-readme
git branch -a
git log --oneline --graph --all

# Regelmäßige Updates und Synchronisation
git checkout main
git pull origin main
git checkout dev
git push origin dev
git merge main
git branch -a
git log --oneline --graph --all
```

## Mitwirken

Pull Requests sind willkommen. Für größere Änderungen öffnen Sie bitte zuerst ein Issue, um zu besprechen, was Sie ändern möchten.


## Lizenz

[MIT](https://choosealicense.com/licenses/mit/)


## Kontakt

Jan Unger – [Website](https://bw-ju.de/) – esel573@gmail.com

Projektlink: <https://github.com/ju1-eu/hello-world>


