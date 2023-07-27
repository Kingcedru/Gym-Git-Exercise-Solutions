# Git exercise project

The project will be used for series of git exercises

## Bundle 1

### Exercise 1

PS C:\Users\The gym\Desktop\git> git status
On branch main

No commits yet

nothing to commit (create/copy files and use "git add" to track)PS C:\Users\The gym\Desktop\git>


                                 git status
No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)        readme.md

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\The gym\Desktop\git> git status       
On branch main

No commits yet
  (use "git rm --cached <file>..." to unstage)
        new file:   readme.md

PS C:\Users\The gym\Desktop\git> git commit -m "init project"   
[main (root-commit) 48c6872] init project
 1 file changed, 2 insertions(+)
 create mode 100644 readme.md
PS C:\Users\The gym\Desktop\git> git remote add origin https://github.com/Kingcedru/Gym-Git-Exercise-Solutions.git
PS C:\Users\The gym\Desktop\git> git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)    
  (use "git restore <file>..." to discard changes in working directory)
        modified:   readme.md

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\The gym\Desktop\git> git commit -m "init project"   
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)    
ectory)
        modified:   readme.md

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\The gym\Desktop\git> git add readme.md
PS C:\Users\The gym\Desktop\git> git commit -m "init project"   
[main e7d8811] init project
 1 file changed, 1 insertion(+)
PS C:\Users\The gym\Desktop\git> git push

    git push --set-upstream origin main

g
upstream, see 'push.autoSetupRemote' in 'git help config'.      

PS C:\Users\The gym\Desktop\git> ^C
PS C:\Users\The gym\Desktop\git> git push --set-upstream origin 
main
fatal: unable to access 'https://github.com/Kingcedru/Gym-Git-Exercise-Solutions.git/': Could not resolve host: github.com      
PS C:\Users\The gym\Desktop\git> git push --set-upstream origin 
Enumerating objects: 6, done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (6/6), 550 bytes | 275.00 KiB/s, done.    
Total 6 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Kingcedru/Gym-Git-Exercise-Solutions.git  
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
PS C:\Users\The gym\Desktop\git> git checkout -b dev
PS C:\Users\The gym\Desktop\git> git push origin dev
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:  
remote:      https://github.com/Kingcedru/Gym-Git-Exercise-Solutions/pull/new/dev
remote:
To https://github.com/Kingcedru/Gym-Git-Exercise-Solutions.git  
 * [new branch]      dev -> dev
PS C:\Users\The gym\Desktop\git> git checkout -b test
PS C:\Users\The gym\Desktop\git> git push origin test
remote:
remote:      https://github.com/Kingcedru/Gym-Git-Exercise-Solutions/pull/new/test
remote:
To https://github.com/Kingcedru/Gym-Git-Exercise-Solutions.git
 * [new branch]      test -> test
PS C:\Users\The gym\Desktop\git> git checkout dev
Switched to branch 'dev'
PS C:\Users\The gym\Desktop\git> git branch -D test
Deleted branch test (was e7d8811).
PS C:\Users\The gym\Desktop\git> git push origin --delete test
To https://github.com/Kingcedru/Gym-Git-Exercise-Solutions.git
 - [deleted]         test
PS C:\Users\The gym\Desktop\git>

### Exercise 2


The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

nothing added to commit but untracked files present (use "git add" to track)

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
$ git stash list

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
$ git add home.html

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
$ git status
On branch dev
Changes to be committed:


IP on dev: e7d8811 init project

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
$ git stash list
stash@{0}: WIP on dev: e7d8811 init project

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
$ git add about.html

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
$ git stash
Saved working directory and index state WIP on dev: e7d8811 init project

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)                               ' can't be assumed due 
$ git stash list
stash@{0}: WIP on dev: e7d8811 init project                                       /git (dev)
stash@{1}: WIP on dev: e7d8811 init project                                       ct
                                         ct
The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)                               /git (dev)
$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in 
what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)      

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
$ git add team.html

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
$ git stash
Saved working directory and index state WIP on dev: e7d8811 init project

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
$ git stash list
stash@{0}: WIP on dev: e7d8811 init project
stash@{1}: WIP on dev: e7d8811 init project
stash@{2}: WIP on dev: e7d8811 init project

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
$ git stash pop stash@{1}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (4bb5a7b7c014c4ed5d8bbb1216069603ca91abe0)

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
$ git stash list
stash@{0}: WIP on dev: e7d8811 init project
stash@{1}: WIP on dev: e7d8811 init project

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
$ git stash pop stash@{1}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (b336c092ea2c62af44ae13db313f7b6ef006a251)

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
$ git add .

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
$ \git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html


The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
$ git commit -m "setup"
[dev 5a4b293] setup
 2 files changed, 22 insertions(+)       
 create mode 100644 about.html
 create mode 100644 home.html

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
$ git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev   

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
$ git push --set-upstream origin dev
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads  
Compressing objects: 100% (4/4), done.   
Writing objects: 100% (4/4), 542 bytes | 
180.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/Kingcedru/Gym-Git-Exercise-Solutions.git
   e7d8811..5a4b293  dev -> dev
branch 'dev' set up to track 'origin/dev'.

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

nothing to commit, working tree clean

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
$ git stash list
stash@{0}: WIP on dev: e7d8811 init project

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
$ git stash pop stash@{0}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped stash@{0} (ad54e026eb564c864464fc7365a1ef532e8cfd67)

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
$ git rest --hard
git: 'rest' is not a git command. See 'git --help'.

The most similar commands are
        restore
        reset

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
v'.

        new file:   team.html


The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
$ git reset --hard
HEAD is now at 5a4b293 setup

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

nothing to commit, working tree clean

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
$
