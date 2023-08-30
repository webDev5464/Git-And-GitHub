# Git Command's

## install git 
[![AGPL License](https://img.shields.io/badge/Site-Git_Download-red.svg)](https://git-scm.com/downloads)

## init

```cmd
git init
```
For Create new empty repository repo.

## status

```cmd
git status
```

Check files status 

- **`untracked files`** : not added for commit file.
- **`changes to be commited`** : your file is ready to commited

```terminal
git status -s
```

easy reed result.

#### How to chack git status ?

*create new file end check git status*

- `untracked files` : new file not added.
- `modified` : change somthing in this file end update to be 
committed.

## add

```cmd
git add
```

untracked file add to tracked *ready for commited.*

### add all untracked file 
```cmd
git add -A
```
new file, modified file & untracked *all types* add to commit.

### add specific file
```cmd
git add demo.html
```
*this command for* : modified file, new file.

## commit

```cmd
git commit
```

|Terminal result|
|:-|

```cmd
[]
#Please enter the commit message for your changes. Lines starting
#with '#' will be ignored, and an empty message aborts the commit.
#
# On branch master
#
# Initial commit
#
# Changes to be committed:
#       new file:   README.md
.git/COMMIT_EDITMSG [unix] (20:40 06/08/2023)                         1,0-1 Top
"~/OneDrive/Desktop/Git Learn/.git/COMMIT_EDITMSG" [unix] 15L, 315Bm
```
- press `i` end write commit message.

```cmd
first git commit
# Please enter the commit message for your changes. Lines starting
# with '#' will be ignored, and an empty message aborts the commit.
#
# On branch master
#
# Initial commit
#
# Changes to be committed:
#       new file:   README.md
.git/COMMIT_EDITMSG[+] [unix] (20:40 06/08/2023)                        1,17 Top-- INSERT --
```

- press `esc` end before press `:` end write `wq` : *enter*
```terminal
delete about file
# Please enter the commit message for your changes. Lines starting      
# with '#' will be ignored, and an empty message aborts the commit.        
#
# On branch master
# Changes to be committed:
#       deleted:    about.html
#
~
~
~
~
.git/COMMIT_EDITMSG[+] [unix] (21:29 06/08/2023)                   
1,17 All:wq
```

your git commit is committed. ✅

**Thiscommiting method is very long method. let's try to sort method.**

```terminal
git commit -m "Add all files"
```

#### How to add also commit end commited message only one command ?

```terminal
git commit -a -m "All file add end commited"
```

## checkout
```terminal
git checkout
``` 
`M index.html` -> modified file.

-> Modifieded file show.

```terminal
git checkout index.html
```

-> Remove modifided changes.
-> Reset last `add` and `commit` changes.

#### How to checkout all modifided files ?

```terminal
git checkout -f
```

## log

```terminal
git log
```

Check commit history

#### log filter

```terminal
git log -p
```

show what is changes commited file

```terminal
git log -p -3
```

`-3` -> 3 commit history show with changes.

## diff

This command only use working directory. If any changes in file end `add`, `commit` than not show any result.

```terminal
git diff
```

Also check specific file.

```terminal
git diff index.html
```

**Last commited file cheack.**

```terminal
git diff --staged
```

## Cheack list all files in directory.

```terminal
ls
```
|Result|
|:-|
|contact.html, index.html,  information.txt,  README.md|

## touch
`touch demo.txt`

For create new file.
*(this command only support git terminal.)*

## rm *(for remove file)*

```terminal
git rm --cached demo.txt
```

delete in commited file

```terminal
rm demo.html
```

delete in directory.

## .gitignore file

- create `.gitignore` file 
```cmd
touch .gitignore
```

#### What is .gitignore file ?
| Ignore File end Folder | Meaning |
|:-|:-|
| demo.html | Not add this file in perent folder. |
| /demo.html | perent folder inside created file ignore. *(tree ingore file)* |
| *.txt | ignore all txt file's |
| demo/ | ignore directory *folder* |

## branch

- `master` :- the master branch is by defult created branch & main branch. Every final work in this branch commit end push.

**cheack branch.**
```cmd
git branch
```

#### How to create new branch ?

```cmd
git branch DemoBranch
```

cheack branches

```cmd
git branch
```

| result |
|:-|
| * master |
| DemoBranch |

`* master` selected branch

#### Switch branch

```cmd
git checkout DemoBranch
```

| result |
|:-|
|  master |
| * DemoBranch |

#### Whay use branches ?

**(1)** : Some changes anything in `DemoBranch` end commit beffore cheack status.

**(2)** : Switch `master` branch. not change here in *master* branch.

#### How to merge another branch with main branch ?

**(1)** : if you are in `anotherBranch` go to `master` branch.

```cmd
git merge DemoBranch
```

***
[![Make Perfect README.md file](https://img.shields.io/badge/Site-readme.so-red.svg)](https://readme.so/) [![Learn : Next Js Documentation](https://img.shields.io/badge/LEARN-Next_js-emreld.svg)](https://github.com/badshah5464/Next_Js-README.git) [![Learn : JavaScript Basic](https://img.shields.io/badge/LEARN-JavaScript_Basic-emreld.svg)](https://github.com/badshah5464/JavaScript-README.git)
***