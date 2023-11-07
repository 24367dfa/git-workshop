---
marp: true
theme: gaia
class:
  - lead
  - invert
paginate: true
headingDivider: 2
---

# n39 Workshop .git



## Was ist git?

- VCS - Version Control System
- ist auf Linux Torvalds Mist gewachsen - für Entwicklung von Linux
- vorallem für Source Code
- funktioniert aber für jegliche plaintext files
- inzwischen das am weitesten verbreitete VCS tool - Industriestandard

## Warum will man das benutzen?

- nie wieder `my_project_version12.zip`, `my_project_version12_final.zip`, `my_project_version12_final_jetzt_aber_wirklich.zip`
- Ausprobieren ohne Angst
- Zusammenarbeit mit anderen
- "Backups" von Software-Projekten

## Basics: Create

```
mkdir my_awesome_repo && cd my_awesome_repo
git init
touch README.md
git add README.md
git commit -m "initial commit"
```

## remote Repositories

```
git remote set-url origin git@github.com:24367dfa/my_awesome_repo.git
git push -u origin main 
```

## Einschub: SSH Key

```
ssh-keygen -t ed_25519 -f .ssh/id_workshop
# bei github hinterlegen https://github.com/settings/keys
```

## Einschub: git config

```
git config --set --global user.email=david.kilias@gmail.com
git config --set --global user.name=David Kilias
```

## Einschub: Nutzt Werkzeuge

- das geht alles auf CLI
- für die Grundlagen und bei Problemen super sinnvoll, das zu beherrschen
- für alle ernstzunehmenden Code Editoren/IDE gibt es Plugins

## Branches

## Log

## Merge

## Rebase

## Reset

## github

- Social Network für Entwickler
- Hosted git mit Drumherum
- wiki, diskussionen, issue tracker, CI, ...

## github: Pullrequests

## github: Actions (CI)