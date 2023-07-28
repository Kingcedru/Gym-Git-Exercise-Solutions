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

## Bundle 2

### Exercise 1


The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

nothing added to commit but untracked fild" to track)

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop
$ git stash list

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop
$ git add home.html

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop
$ git status
On branch dev
Changes to be committed:


IP on dev: e7d8811 init project

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop
$ git stash list
stash@{0}: WIP on dev: e7d8811 init proje

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop
$ git add about.html

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop
$ git stash
Saved working directory and index state W project

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop
The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
$ git stash list
stash@{0}: WIP on dev: e7d8811 init project
stash@{1}: WIP on dev: e7d8811 init project

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
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

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop
$ git stash list
stash@{0}: WIP on dev: e7d8811 init proje

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop
$ git stash pop stash@{0}
On branch dev
Your branch is up to date with 'origin/de

Changes to be committed:
  (use "git restore --staged <file>..." t
        new file:   team.html

Dropped stash@{0} (ad54e026eb564c864464fc

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop
$ git rest --hard
git: 'rest' is not a git command. See 'gi

The most similar commands are
        restore
        reset

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop
v'.

        new file:   team.html


The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop
$ git reset --hard

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (dev)
$ git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/bundle-2)
$ git status
On branch ft/bundle-2
nothing to commit, working tree clean

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/bundle-2)
$ git status
On branch ft/bundle-2
Untracked files:
  (use "git add <file>..." to include in 
what will be committed)
        service.html

nothing added to commit but untracked files present (use "git add" to track)      

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/bundle-2)
$ git add service.html

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/bundle-2)
$ git stash
Saved working directory and index state WIP on ft/bundle-2: 5a4b293 setup

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/bundle-2)
$ git stash pop
On branch ft/bundle-2
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   service.html

Dropped refs/stash@{0} (23efda7c71e26ed3ebb466f554aae2b4e9814db7)

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/bundle-2)
$ git status
On branch ft/bundle-2
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   service.html


The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/bundle-2)
$ git add service.html

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/bundle-2)
$ git commit -m "create service page"
[ft/bundle-2 18a1648] create service page 1 file changed, 11 insertions(+)        
 create mode 100644 service.html

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/bundle-2)
$ git push
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/bundle-2)
$ git push --set-upstream origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads  
Compressing objects: 100% (3/3), done.   
Writing objects: 100% (3/3), 455 bytes | 
455.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/Kingcedru/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2
To https://github.com/Kingcedru/Gym-Git-Exercise-Solutions.git     
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.        

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/bundle-2)        
$

### Exercise 2

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop
/git (ft/bundle-2)
$ git status
On branch ft/bundle-2
Changes to be committed:
  (use "git restore --staged <file>..." t
o unstage)
        new file:   service.html


The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop
/git (ft/bundle-2)
$ git add service.html

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop
/git (ft/bundle-2)
$ git commit -m "create service page"
[ft/bundle-2 18a1648] create service page
 1 file changed, 11 insertions(+)        
 create mode 100644 service.html

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop
/git (ft/bundle-2)
$ git push
fatal: The current branch ft/bundle-2 has
 no upstream branch.
To push the current branch and set the re
mote as upstream, use

    git push --set-upstream origin ft/bun
dle-2

To have this happen automatically for bra
nches without a tracking
upstream, see 'push.autoSetupRemote' in '
git help config'.


The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop
/git (ft/bundle-2)
$ git push --set-upstream origin ft/bundl
e-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads  
Compressing objects: 100% (3/3), done.   
Writing objects: 100% (3/3), 455 bytes | 
455.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pa
ck-reused 0
remote: Resolving deltas: 100% (1/1), com
pleted with 1 local object.
remote:
remote: Create a pull request for 'ft/bun
dle-2' on GitHub by visiting:
remote:      https://github.com/Kingcedru
/Gym-Git-Exercise-Solutions/pull/new/ft/b
undle-2
remote:
To https://github.com/Kingcedru/Gym-Git-Exercise
To https://github.com/Kingcedru/Gym-Git-Exercise
 * [new branch]      ft/bundle-2 -> ft/bundle-2
To https://github.com/Kingcedru/Gym-Git-Exercise
To https://github.com/Kingcedru/Gym-Git-Exercise
To https://github.com/Kingcedru/Gym-Git-Exercise

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/bundle-2)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (main)      
$ git checkout -b ft/service-redesign

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/service-redesigngit (ft/service-redesign)
$ git status
On branch ft/service-redesign
nothing to commit, working tree clean     
                                          git (ft/service-redesign
The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/service-redesign)
$ git checkout -D ft/service-redesign
error: unknown switch `D'
usage: git checkout [<options>] <branch>
   or: git checkout [<options>] [<branch>] -- <file>...

    -b <branch>           create and checkout a new branch
    -B <branch>           create/reset and checkout a branch
    -l                    create reflog for new branch
    --guess               second guess 'git checkout <no-such-branch>' (default)    
    --overlay             use overlay mode (default)
    -q, --quiet           suppress progress reporting
    --recurse-submodules[=<checkout>]     
                          control recursive updating of submodules
    --progress            force progress reporting
    -m, --merge           perform a 3-way 
merge with the new branch
    --conflict <style>    conflict style (merge, diff3, or zdiff3)
    -d, --detach          detach HEAD at named commit
    -t, --track[=(direct|inherit)]        
                          set branch tracking configuration
    -f, --force           force checkout (throw away local modifications)
    --orphan <new-branch>
                          new unparented branch
    --overwrite-ignore    update ignored files (default)
    --ignore-other-worktrees
                          do not check if 
another worktree is holding the given ref 
    -2, --ours            checkout our version for unmerged files
    -3, --theirs          checkout their version for unmerged files
    -p, --patch           select hunks interactively
    --ignore-skip-worktree-bits
                          do not limit pathspecs to sparse entries only
    --pathspec-from-file <file>
                          read pathspec from file
    --pathspec-file-nul   with --pathspec-from-file, pathspec elements are separated with NUL character


The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (main)
$ git pull
remote: Enumerating objects: 15, done.    
remote: Counting objects: 100% (14/14), done.
remote: Compressing objects: 100% (8/8), done.
remote: Total 11 (delta 3), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (11/11), 4.62 KiB 
| 68.00 KiB/s, done.
From https://github.com/Kingcedru/Gym-Git-Exercise-Solutions
   e7d8811..05f150d  main       -> origin/main
Updating e7d8811..05f150d
Fast-forward
 about.html   |  11 ++
 home.html    |  11 ++
 readme.md    | 537 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-     

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (main)
$ git checkout -b ft/service-redesign
fatal: a branch named 'ft/service-redesign' already exists

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (main)
$ git checkout -D ft/service-redesign
error: unknown switch `D'
usage: git checkout [<options>] <branch>
   or: git checkout [<options>] [<branch>] -- <file>...

    -b <branch>           create and checkout a new branch
    -B <branch>           create/reset and checkout a branch
    -l                    create reflog for new branch
    --guess               second guess 'git checkout <no-such-branch>' (default)    
    --overlay             use overlay mode (default)
    -q, --quiet           suppress progress reporting
    --recurse-submodules[=<checkout>]     
                          control recursive updating of submodules
    --progress            force progress reporting
    -m, --merge           perform a 3-way 
merge with the new branch
    --conflict <style>    conflict style (merge, diff3, or zdiff3)
    -d, --detach          detach HEAD at named commit
    -t, --track[=(direct|inherit)]        
                          set branch tracking configuration
    -f, --force           force checkout (throw away local modifications)
    --orphan <new-branch>
                          new unparented branch
    --overwrite-ignore    update ignored files (default)
    --ignore-other-worktrees
                          do not check if 
another worktree is holding the given ref 
    -2, --ours            checkout our version for unmerged files
    -3, --theirs          checkout their version for unmerged files
    -p, --patch           select hunks interactively
    --ignore-skip-worktree-bits
                          do not limit pathspecs to sparse entries only
    --pathspec-from-file <file>
                          read pathspec from file
    --pathspec-file-nul   with --pathspec-from-file, pathspec elements are separated with NUL character


The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (main)
$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/service-redesign)
$ git add .

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/service-redesign)
$ git status
On branch ft/service-redesign
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   service.html


The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/service-redesign)
$ git commit -m "service list"
[ft/service-redesign ec33880] service list 1 file changed, 7 insertions(+)

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/service-redesign)
$ git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/service-redesign)
$ git push --set-upstream origin ft/service-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads   
Compressing objects: 100% (3/3), done.    
Writing objects: 100% (3/3), 342 bytes | 342.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote: 
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:      
remote:      https://github.com/Kingcedru/Gym-Git-Exercise-Solutions/pull/new/ft/service-redesign
remote:
To https://github.com/Kingcedru/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (main)
$  git commit -m "old services"
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)      
  (use "git restore <file>..." to discard changes in working directory)
        modified:   service.html

no changes added to commit (use "git add" and/or "git commit -a") 

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)      
  (use "git restore <file>..." to discard changes in working directory)
        modified:   service.html

no changes added to commit (use "git add" and/or "git commit -a") 

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (main)
$ git add .

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (main)
$  git commit -m "old services"
[main cb199f7] old services
 1 file changed, 8 insertions(+), 1 deletion(-)

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 355 bytes | 355.00 KiB/s, done.      
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Kingcedru/Gym-Git-Exercise-Solutions.git    
   05f150d..cb199f7  main -> main

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (main)
$ git checkout ft/service

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.
