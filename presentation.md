---
marp: true
theme: gaia
class:
  - lead
  - invert
paginate: true
headingDivider: 2
---

# n39 Workshop - git

2023-11-22
David
https://github.com/24367dfa

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

## Basics: `git init`

```bash
mkdir my_awesome_repo && cd my_awesome_repo
git init
touch README.md
git add README.md
git commit -m "initial commit"
```

## Basics: `git status`

```bash
git status
```

## Einschub: `git config`

```bash
git config --set --global user.email="david.kilias@gmail.com"
git config --set --global user.name="David Kilias"
```

## Basics: `git branch`

```bash
git branch
git branch my-test-branch
git checkout my-test-branch
git checkout main
git branch -d my-test-branch
```

## Basics: `git remote`

```bash
git remote set-url origin git@github.com:24367dfa/my_awesome_repo.git
git push -u origin main 
```

ein Repository kann mehr als ein remote haben

## Einschub: SSH Key

```bash
ssh-keygen -t ed_25519 -f ~/.ssh/id_workshop
cat ~/.ssh/id_workshop.pub | xclip -selection c
```

bei github hinterlegen https://github.com/settings/keys

## Basics: Zusammenfassung

![height:500px](img/git-commands.png)

## Einschub: Nutzt Werkzeuge

- das geht alles auf CLI
- für die Grundlagen und bei Problemen super sinnvoll, das zu beherrschen
- für alle ernstzunehmenden Editoren/IDE gibt es Plugins

## Intermediate: `git log`

```
git log
git log -5
git log -L 1,10:README.md
```

## Advanced: `git rebase` vs `git merge`

![height:500px](img/git-merge-git-rebase.jpeg)

## Reset

## github

- Social Network für Entwickler
- Hosted git mit Drumherum
- wiki, diskussionen, issue tracker, CI, ...

## github: Pullrequests

- Review
- Fork
- 

## github: Actions (CI/CD)

## Links

(git docs)[https://git-scm.com/docs]
(oh-shit-git)[https://ohshitgit.com/]

## Bildquellen

[bytebytego.com](https://github.com/ByteByteGoHq/system-design-101#git)

## Lizenz

[![License: CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/)