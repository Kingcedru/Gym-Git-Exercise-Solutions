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
