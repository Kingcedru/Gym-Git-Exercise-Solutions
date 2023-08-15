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

## Bundle 3

### Exercise 1


The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git
$ git checkout main
Switched to branch 'main'
Your branch and 'origin/main' have diverged,
and have 1 and 4 different commits each, resp
  (use "git pull" to merge the remote branch 

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git
$ git branch -D ft/team-page
Deleted branch ft/team-page (was 6585e4e).

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git
$ git branch -D ft/contact-page
Deleted branch ft/contact-page (was 0150327).

 - [deleted]         ft/contact-page       

xercise-Solutions.git                    /git
 - [deleted]         ft/team-page        
                                         xerc
The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (main)
$ git checkout -b ft/team-page           /git
Switched to a new branch 'ft/team-page'  

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/team-page)                      /git
$ git add team.html

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/team-page)
$ git commit "team.html file"
error: pathspec 'team.html file' did not 
match any file(s) known to git

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/team-page)
$ git commit -m "team.html file"
[ft/team-page 552f4c7] team.html file
 1 file changed, 11 insertions(+)
 create mode 100644 team.html

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/team-page)
$ git push
fatal: The current branch ft/team-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/team-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/team-page)
$ git push --set-upstream origin ft/team-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 445 bytes | 445.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.       
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:    
remote:      https://github.com/Kingcedru/Gym-Git-Exercise-Solutions/pull/new/ft/team-page
remote:
To https://github.com/Kingcedru/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/team-page)
$ git checkout main
error: Your local changes to the following files would be overwritten by checkout:
        team.html
Please commit your changes or stash them before you switch branches.       
Aborting

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/team-page)
$ git status
On branch ft/team-page
Your branch is up to date with 'origin/ft/team-page'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)    
        modified:   team.html

no changes added to commit (use "git add" and/or "git commit -a")

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/team-page)
$ git push --set-upstream origin ft/team-page
Everything up-to-date
branch 'ft/team-page' set up to track 'origin/ft/team-page'.

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/team-page)
$ git status
On branch ft/team-page
Your branch is up to date with 'origin/ft/team-page'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)    
        modified:   team.html

no changes added to commit (use "git add" and/or "git commit -a")

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/team-page)
$ git add team.html

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/team-page)
$ git commit -m "team.html file"
[ft/team-page a0aad99] team.html file
 1 file changed, 1 insertion(+), 1 deletion(-)

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/team-page)
$ git push --set-upstream origin ft/team-page
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 285 bytes | 285.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.      
To https://github.com/Kingcedru/Gym-Git-Exercise-Solutions.git
   552f4c7..a0aad99  ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/team-page)
$ git status
On branch ft/team-page
Your branch is up to date with 'origin/ft/team-page'.

nothing to commit, working tree clean

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/team-page)
$ git checkout main
Switched to branch 'main'
Your branch and 'origin/main' have diverged,
and have 1 and 4 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (main)
$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/contact-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/team-page)
$ git log
commit a0aad9977fe35bf6f8a31ac1c8a19e81af9e64d6 (HEAD -> ft/team-page, origin/ft/team-page)
Author: cedrick byishimo <byishimocedrick@gmail.com>
Date:   Thu Aug 3 08:53:41 2023 +0200

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/contact-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/team-page)
$ git log
commit a0aad9977fe35bf6f8a31ac1c8a19e81af9e64d6 (HEAD -> ft/team-page, origin/ft
/team-page)
Author: cedrick byishimo <byishimocedrick@gmail.com>
Date:   Thu Aug 3 08:53:41 2023 +0200

    team.html file

commit 552f4c7d2a9833f0d9ad1ae63fa38d756f59d57e
Author: cedrick byishimo <byishimocedrick@gmail.com>
Date:   Thu Aug 3 08:51:11 2023 +0200

    team.html file

commit 00b5e5fd2e5cfb6c47c3b94b5e341b97e160bbdb (main, ft/contact-page)
Author: cedrick byishimo <byishimocedrick@gmail.com>
Date:   Tue Aug 1 12:34:24 2023 +0200

    changes

commit cb199f7ee832dc8d1e991a522d9be26af1f06390
Author: cedrick byishimo <byishimocedrick@gmail.com>
Date:   Fri Jul 28 11:20:30 2023 +0200


The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/contact-page)
$ git cherry-pick a0aad9977fe35bf6f8a31ac1c8a19e81af9e64d6
CONFLICT (modify/delete): team.html deleted in HEAD and modified in a0aad99 (tea
m.html file).  Version a0aad99 (team.html file) of team.html left in tree.
error: could not apply a0aad99... team.html file
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git cherry-pick --continue".
hint: You can instead skip this commit with "git cherry-pick --skip".
hint: To abort and get back to the state before "git cherry-pick",
hint: run "git cherry-pick --abort".

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/contact-page|CHERRY-PICKING)
$ vi team.html

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/contact-page|CHERRY-PICKING)
$ vi team.html

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/contact-page|CHERRY-PICKING)
$ git cherry-pick --abort

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/contact-page)
$ git status
On branch ft/contact-page
nothing to commit, working tree clean

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/contact-page)
$ git add .

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/contact-page)
$ git commmit -m "cherry-pick"
git: 'commmit' is not a git command. See 'git --help'.

The most similar command is
        commit

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/contact-page)
$ git commit -m "cherry-pick"
On branch ft/contact-page
nothing to commit, working tree clean

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/contact-page)
$ git push
fatal: The current branch ft/contact-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/contact-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/contact-page)
$ git push --set-upstream origin ft/contact-page
error: unable to read askpass response from 'C:/Program Files/Git/mingw64/bin/git-askpass.exe'
Password for 'https://Kingcedru@github.com':
remote: Invalid username or password.
fatal: Authentication failed for 'https://github.com/Kingcedru/Gym-Git-Exercise-Solutions.git/'

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/contact-page)
$ git config --global user.name "Kingcedru"

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/contact-page)
$ git config --global user.email "byishimocedrick@gmail.com"

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/contact-page)
$ git push --set-upstream origin ft/contact-page
error: unable to read askpass response from 'C:/Program Files/Git/mingw64/bin/git-askpass.exe'
Username for 'https://github.com':
error: unable to read askpass response from 'C:/Program Files/Git/mingw64/bin/git-askpass.exe'
Password for 'https://github.com':
remote: No anonymous write access.
fatal: Authentication failed for 'https://github.com/Kingcedru/Gym-Git-Exercise-Solutions.git/'


The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/contact-page)
$

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/contact-page)
$ git push origin ft/contact-page
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/Kingcedru/Gym-Git-Exercise-Solutions/pull/new/ft/contact-page
remote:
To https://github.com/Kingcedru/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/contact-page)
$ ^C

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/contact-page)
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/faq-page)
$ git status
On branch ft/faq-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        faq.html

nothing added to commit but untracked files present (use "git add" to track)

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/faq-page)
$ git add .

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/faq-page)
$ git commit -m "faq.html page"
[ft/faq-page 300a540] faq.html page
 1 file changed, 11 insertions(+)
 create mode 100644 faq.html

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/faq-page)
$ git push
fatal: The current branch ft/faq-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/faq-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/faq-page)
$ ^[[200~
bash: $'\E[200~': command not found

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/faq-page)
$ git push --set-upstream origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 435 bytes | 435.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/Kingcedru/Gym-Git-Exercise-Solutions/pull/new/ft/faq-page
remote:
To https://github.com/Kingcedru/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/faq-page)
$ git revert a0aad9977fe35bf6f8a31ac1c8a19e81af9e64d6
Auto-merging faq.html
On branch ft/faq-page
Your branch is up to date with 'origin/ft/faq-page'.

nothing to commit, working tree clean

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/faq-page)
$ git add .

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/faq-page)
$ git commit -m "reverted"
On branch ft/faq-page
Your branch is up to date with 'origin/ft/faq-page'.

nothing to commit, working tree clean

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (ft/faq-page)
$ git push
Everything up-to-date

The gym@DESKTOP

## Bundle 4
### Exercise 1

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (main)
$ git checkout main
Already on 'main'
Your branch and 'origin/main' have diverged,
and have 2 and 4 different commits each, respectively.  
  (use "git pull" to merge the remote branch into yours)

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (main)
$ git remotes add git-copy https://github.com/Kingcedru/Gym-Git-Exercise-Solutions-cloned.git
git: 'remotes' is not a git command. See 'git --help'.

The most similar command is
        remote

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (main)

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (main)
$ git remote
git-copy
origin

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (main)
$ git status
On branch main
Your branch and 'origin/main' have diverged,
and have 2 and 4 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)        

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)    
  (use "git restore <file>..." to discard changes in working directory)
        modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (main)
$ git add .

The gym@DESKTOP-KAP26A5 MINGW64 ~/Desktop/git (main)
$ git commit -m "add icon"
[main c5b9a8d] add icon
 1 file changed, 1 insertion(+)
The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git (main)
$ git push
Enumerating objects: 12, done.
Counting objects: 100% (12/12), done.
Delta compression using up to 4 threads
Compressing objects: 100% (8/8), done.
Writing objects: 100% (8/8), 883 bytes | 883.00 KiB/s, done.
Total 8 (delta 5), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (5/5), completed with 3 local objects.
To https://github.com/Kingcedru/Gym-Git-Exercise-Solutions.git
   c89d879..225c72c  main -> main

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git (main)
$ git push git-copy
Enumerating objects: 54, done.
Counting objects: 100% (54/54), done.
Delta compression using up to 4 threads
Compressing objects: 100% (49/49), done.
Writing objects: 100% (54/54), 14.61 KiB | 2.09 MiB/s, done.
Total 54 (delta 23), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (23/23), done.
To https://github.com/Kingcedru/Gym-Git-Exercise-Solutions-cloned.git
 * [new branch]      main -> main

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git (main)
$ git push origin
Everything up-to-date

### Exercise 2

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git (main)
$ git checkout ft/footer
error: pathspec 'ft/footer' did not match any file(s) known to git

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git (main)
$ git checkout -b ft/footer
Switched to a new branch 'ft/footer'

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git (ft/footer)
$ git add footer.html

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git (ft/footer)
$ git commit -m "footer.html first commit"
[ft/footer ba55063] footer.html first commit
 1 file changed, 11 insertions(+)
 create mode 100644 footer.html

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git (ft/footer)
$ git add footer.html

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git (ft/footer)
$ git commit -m "footer.html second commit"
[ft/footer cb25d5c] footer.html second commit
 1 file changed, 3 insertions(+)

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git (ft/footer)
$ git push
fatal: The current branch ft/footer has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/footer

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git (ft/footer)
$  git push --set-upstream origin ft/footer
Enumerating objects: 30, done.
Counting objects: 100% (28/28), done.
Delta compression using up to 4 threads
Compressing objects: 100% (21/21), done.
Writing objects: 100% (21/21), 6.47 KiB | 1.62 MiB/s, done.
Total 21 (delta 11), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (11/11), completed with 3 local objects.
remote:
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:      https://github.com/Kingcedru/Gym-Git-Exercise-Solutions/pull/new/ft
/footer
remote:
To https://github.com/Kingcedru/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/footer -> ft/footer
branch 'ft/footer' set up to track 'origin/ft/footer'.

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git (ft/footer)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git (main)
$ git checkout -b ft/sqashing
Switched to a new branch 'ft/sqashing'

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git (ft/sqashing)
$ git merge --squash ft/footer
Updating 225c72c..cb25d5c
Fast-forward
Squash commit -- not updating HEAD
 footer.html | 14 ++++++++++++++
 1 file changed, 14 insertions(+)
 create mode 100644 footer.html

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git (ft/sqashing)
$ git commit -m "footer changes squashing"
[ft/sqashing febedbb] footer changes squashing
 1 file changed, 14 insertions(+)
 create mode 100644 footer.html

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git (ft/sqashing)
$ git push
fatal: The current branch ft/sqashing has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/sqashing

## Bundle 5

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git (ft/sqashing)
$ ^[[200~
bash: $'\E[200~': command not found

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git (ft/sqashing)
$ git push --set-upstream origin ft/sqashing
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 472 bytes | 472.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/sqashing' on GitHub by visiting:
remote:      https://github.com/Kingcedru/Gym-Git-Exercise-Solutions/pull/new/ft
/sqashing
remote:
To https://github.com/Kingcedru/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/sqashing -> ft/sqashing
branch 'ft/sqashing' set up to track 'origin/ft/sqashing'.

## Bundle 5
### Exercise 1

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git (ft/sqashing)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git (main)
$ git pull
remote: Enumerating objects: 8, done.
remote: Counting objects: 100% (8/8), done.
remote: Compressing objects: 100% (6/6), done.
remote: Total 6 (delta 4), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (6/6), 2.26 KiB | 55.00 KiB/s, done.
From https://github.com/Kingcedru/Gym-Git-Exercise-Solutions
   225c72c..cc9c1d1  main       -> origin/main
Updating 225c72c..cc9c1d1
Fast-forward
 readme.md | 188 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 1 file changed, 188 insertions(+)

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git (main)
$ git add index.html

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git (main)
$ git add home.html

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git (main)
$ git commit -m "renamed"
[main a8c5401] renamed
 1 file changed, 0 insertions(+), 0 deletions(-)
 rename home.html => index.html (100%)

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git (main)
$ git push
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 231 bytes | 231.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Kingcedru/Gym-Git-Exercise-Solutions.git
   cc9c1d1..a8c5401  main -> main

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git (main)
$ git push git-copy
Enumerating objects: 10, done.
Counting objects: 100% (10/10), done.
Delta compression using up to 4 threads
Compressing objects: 100% (8/8), done.
Writing objects: 100% (8/8), 2.50 KiB | 1.25 MiB/s, done.
Total 8 (delta 5), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (5/5), completed with 2 local objects.
To https://github.com/Kingcedru/Gym-Git-Exercise-Solutions-cloned.git
   225c72c..a8c5401  main -> main

### Exercise 2

The gym@DESKTOP-KAP26A5 MINGW64 ~ (master)
$ git clone https://github.com/Kingcedru/git-cafe-exercise.git
Cloning into 'git-cafe-exercise'...
remote: Enumerating objects: 107, done.
remote: Counting objects: 100% (14/14), done.
remote: Compressing objects: 100% (10/10), done.
remote: Total 107 (delta 5), reused 4 (delta 4), pack-reused 93
Receiving objects: 100% (107/107), 1.95 MiB | 851.00 KiB/s, done.
Resolving deltas: 100% (5/5), done.

The gym@DESKTOP-KAP26A5 MINGW64 ~ (master)
$ code .

The gym@DESKTOP-KAP26A5 MINGW64 ~ (master)
$ cd ^[[200~
bash: cd: $'\E[200~': No such file or directory

The gym@DESKTOP-KAP26A5 MINGW64 ~ (master)
$ cd git-cafe-exercise
bash: cd: git-cafe-exercise: No such file or directory

The gym@DESKTOP-KAP26A5 MINGW64 ~ (master)
$ cd desktop

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop (master)
$ cd git-cafe-exercise

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git-cafe-exercise (main)
$ code .

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git-cafe-exercise (main)
$ git add index.html

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git-cafe-exercise (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   index.html


The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git-cafe-exercise (main)
$ git commit -m "change title"
[main f0f06d2] change title
 1 file changed, 1 insertion(+), 1 deletion(-)

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git-cafe-exercise (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 319 bytes | 319.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Kingcedru/git-cafe-exercise.git
   d1d3f9c..f0f06d2  main -> main

## BUndle 6
### Exercise 1

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git-cafe-exercise (ft/menu)
$ git checkout -b menu
Switched to a new branch 'menu'

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git-cafe-exercise (menu)
$ git push
fatal: The current branch menu has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin menu

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git-cafe-exercise (menu)
$ git push --set-upstream origin menu
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'menu' on GitHub by visiting:
remote:      https://github.com/Kingcedru/git-cafe-exercise/pull/new/menu
remote:
To https://github.com/Kingcedru/git-cafe-exercise.git
 * [new branch]      menu -> menu
branch 'menu' set up to track 'origin/menu'.

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git-cafe-exercise (menu)
$ git add menu.html

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git-cafe-exercise (menu)
$ git commit -m 'menu page'
[menu 05db3be] menu page
 1 file changed, 11 insertions(+)
 create mode 100644 menu.html

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git-cafe-exercise (menu)
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 439 bytes | 439.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Kingcedru/git-cafe-exercise.git
   f0f06d2..05db3be  menu -> menu

### Exercise 2

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git-cafe-exercise (menu)
$ git checkout -b bugFix
Switched to a new branch 'bugFix'

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git-cafe-exercise (bugFix)
$ git status
On branch bugFix
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   index-4.html

no changes added to commit (use "git add" and/or "git commit -a")

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git-cafe-exercise (bugFix)
$ git add index-4.html

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git-cafe-exercise (bugFix)
$ git commit -m "changed title"
[bugFix 2c1de34] changed title
 1 file changed, 1 insertion(+), 1 deletion(-)

The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git-cafe-exercise (bugFix)
$ git push
fatal: The current branch bugFix has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin bugFix

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


The gym@DESKTOP-KAP26A5 MINGW64 ~/desktop/git-cafe-exercise (bugFix)
$ git push --set-upstream origin bugFix
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 301 bytes | 301.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'bugFix' on GitHub by visiting:
remote:      https://github.com/Kingcedru/git-cafe-exercise/pull/new/bugFix
remote:
To https://github.com/Kingcedru/git-cafe-exercise.git
 * [new branch]      bugFix -> bugFix
branch 'bugFix' set up to track 'origin/bugFix'.
