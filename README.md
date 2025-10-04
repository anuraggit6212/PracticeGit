#### Practicing Github

C:\GitPractice>git status

C:\GitPractice>git add README.md

C:\GitPractice>git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md


C:\GitPractice>git branch

C:\GitPractice>git commit -m "This is my first commit"
[master (root-commit) e9c3cb7] This is my first commit
 1 file changed, 1 insertion(+)
 create mode 100644 README.md

C:\GitPractice>git branch -m Main

C:\GitPractice>git branch
* Main

C:\GitPractice>git remote add origin https://github.com/anuraggit6212/PracticeGit.git

C:\GitPractice>git remote -v
origin  https://github.com/anuraggit6212/PracticeGit.git (fetch)
origin  https://github.com/anuraggit6212/PracticeGit.git (push)

C:\GitPractice>git push origin Main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 242 bytes | 242.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/anuraggit6212/PracticeGit.git
 * [new branch]      Main -> Main

C:\GitPractice>git config --global user.name "Anurag Mahalpure"

C:\GitPractice>git config --global user.email "anuragmahalpure@gmail.com"

C:\GitPractice> git add README.md

C:\GitPractice>git status
On branch Main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md


C:\GitPractice>git commit -m "Second Commit"
[Main 5588394] Second Commit
 1 file changed, 1 insertion(+), 1 deletion(-)

C:\GitPractice>git push origin Main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Writing objects: 100% (3/3), 269 bytes | 269.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/anuraggit6212/PracticeGit.git
   e9c3cb7..5588394  Main -> Main

C:\GitPractice>git status
On branch Main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        app.py

nothing added to commit but untracked files present (use "git add" to track)      

C:\GitPractice>git status  
On branch Main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        app.py
        main.py

nothing added to commit but untracked files present (use "git add" to track)      

C:\GitPractice>git add .

C:\GitPractice>git commit -m "Third Commit"
[Main 7049699] Third Commit
 2 files changed, 2 insertions(+)
 create mode 100644 app.py
 create mode 100644 main.py

C:\GitPractice>git push origin main
fatal: main cannot be resolved to branch

C:\GitPractice>git push origin Main 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (4/4), 345 bytes | 172.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/anuraggit6212/PracticeGit.git
   5588394..7049699  Main -> Main

C:\GitPractice>git pull origin main
fatal: couldn't find remote ref main

C:\GitPractice>git add .

C:\GitPractice>git commit -m
error: switch `m' requires a value

C:\GitPractice>git commit -m "Fourth commit"
[Main 20e05f2] Fourth commit
 1 file changed, 1 insertion(+), 1 deletion(-)

C:\GitPractice>git push origin Main
To https://github.com/anuraggit6212/PracticeGit.git
 ! [rejected]        Main -> Main (fetch first)
error: failed to push some refs to 'https://github.com/anuraggit6212/PracticeGit.git'
hint: Updates were rejected because the remote contains work that you do not      
hint: have locally. This is usually caused by another repository pushing to       
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.        

C:\GitPractice>git status
On branch Main
nothing to commit, working tree clean

C:\GitPractice>git pull origin Main
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 2.85 KiB | 81.00 KiB/s, done.
From https://github.com/anuraggit6212/PracticeGit
 * branch            Main       -> FETCH_HEAD
   7049699..83fa1f8  Main       -> origin/Main
hint: Waiting for your editor to close the file...
Merge made by the 'ort' strategy.
 .gitignore | 207 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 1 file changed, 207 insertions(+)
 create mode 100644 .gitignore

remote: Compressing objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 2.85 KiB | 81.00 KiB/s, done.
From https://github.com/anuraggit6212/PracticeGit
 * branch            Main       -> FETCH_HEAD
   7049699..83fa1f8  Main       -> origin/Main
hint: Waiting for your editor to close the file...
Merge made by the 'ort' strategy.
 .gitignore | 207 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++   
 1 file changed, 207 insertions(+)
 create mode 100644 .gitignore

Unpacking objects: 100% (3/3), 2.85 KiB | 81.00 KiB/s, done.
From https://github.com/anuraggit6212/PracticeGit
 * branch            Main       -> FETCH_HEAD
   7049699..83fa1f8  Main       -> origin/Main
hint: Waiting for your editor to close the file...
Merge made by the 'ort' strategy.
 .gitignore | 207 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++   
 1 file changed, 207 insertions(+)
 create mode 100644 .gitignore

hint: Waiting for your editor to close the file...
Merge made by the 'ort' strategy.
 .gitignore | 207 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++   
 1 file changed, 207 insertions(+)
 create mode 100644 .gitignore

Merge made by the 'ort' strategy.
 .gitignore | 207 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++   
 1 file changed, 207 insertions(+)
 create mode 100644 .gitignore

 .gitignore | 207 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++   
 1 file changed, 207 insertions(+)
 create mode 100644 .gitignore

 1 file changed, 207 insertions(+)
 create mode 100644 .gitignore

 create mode 100644 .gitignore


C:\GitPractice>python -m venv venv


C:\GitPractice>python -m venv venv

C:\GitPractice>python -m venv venv
C:\GitPractice>python -m venv venv


C:\GitPractice>venv/Scripts/Activate
'venv' is not recognized as an internal or external command,
operable program or batch file.

C:\GitPractice>venv\Scripts\Activate

(venv) C:\GitPractice>git add .

(venv) C:\GitPractice>git status
On branch Main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   .gitignore
        modified:   app.py


(venv) C:\GitPractice>git status
On branch Main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   .gitignore
        modified:   app.py

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   .gitignore


(venv) C:\GitPractice>git status
On branch Main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   .gitignore
        modified:   app.py

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   .gitignore

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test/


(venv) C:\GitPractice>git status
On branch Main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   .gitignore
        modified:   app.py

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   .gitignore


(venv) C:\GitPractice>git add .

(venv) C:\GitPractice>git commit -m "Updated Git Ignore"
[Main 5bf3308] Updated Git Ignore
 2 files changed, 8 insertions(+), 1 deletion(-)

(venv) C:\GitPractice>git push origin Main
Enumerating objects: 16, done.
Counting objects: 100% (14/14), done.
Delta compression using up to 12 threads
Compressing objects: 100% (8/8), done.
Writing objects: 100% (9/9), 936 bytes | 234.00 KiB/s, done.
Total 9 (delta 3), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (3/3), completed with 2 local objects.
To https://github.com/anuraggit6212/PracticeGit.git
   83fa1f8..5bf3308  Main -> Main

(venv) C:\GitPractice>git branch
* Main

(venv) C:\GitPractice>git branch developerA

(venv) C:\GitPractice>git branch
* Main
  developerA

(venv) C:\GitPractice>git status
On branch Main
nothing to commit, working tree clean

(venv) C:\GitPractice>git checkout developerA
Switched to branch 'developerA'

(venv) C:\GitPractice>git branch
  Main
* developerA

(venv) C:\GitPractice>git status
On branch developerA
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   app.py

no changes added to commit (use "git add" and/or "git commit -a")

(venv) C:\GitPractice>git add 
Nothing specified, nothing added.
hint: Maybe you wanted to say 'git add .'?
hint: Disable this message with "git config set advice.addEmptyPathspec false"    

(venv) C:\GitPractice>git add .

(venv) C:\GitPractice>git commit -m "developerA story"
[developerA 207aa35] developerA story
 1 file changed, 4 insertions(+), 1 deletion(-)

(venv) C:\GitPractice>git checkout Main
Switched to branch 'Main'

(venv) C:\GitPractice>git merge develoerA  
merge: develoerA - not something we can merge

(venv) C:\GitPractice>git merge developerA
Updating 5bf3308..207aa35
Fast-forward
 app.py | 5 ++++-
 1 file changed, 4 insertions(+), 1 deletion(-)

(venv) C:\GitPractice>git branch -d developerA
Deleted branch developerA (was 207aa35).

(venv) C:\GitPractice>git status
On branch Main
nothing to commit, working tree clean

(venv) C:\GitPractice>git branch
* Main

(venv) C:\GitPractice>git push origin main

(venv) C:\GitPractice>git push origin Main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 320 bytes | 320.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/anuraggit6212/PracticeGit.git
   5bf3308..207aa35  Main -> Main

(venv) C:\GitPractice>git add .                          

(venv) C:\GitPractice>git status
On branch Main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   app.py


(venv) C:\GitPractice>git commit -m "Updated Sub in app"
[Main 75202a3] Updated Sub in app
 1 file changed, 2 insertions(+), 2 deletions(-)

(venv) C:\GitPractice>git push origin Main
To https://github.com/anuraggit6212/PracticeGit.git
 ! [rejected]        Main -> Main (fetch first)
error: failed to push some refs to 'https://github.com/anuraggit6212/PracticeGit.git'
hint: Updates were rejected because the remote contains work that you do not
hint: have locally. This is usually caused by another repository pushing to       
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.        

(venv) C:\GitPractice>git pull origin Main
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 964 bytes | 56.00 KiB/s, done.
From https://github.com/anuraggit6212/PracticeGit
 * branch            Main       -> FETCH_HEAD
   207aa35..243ad76  Main       -> origin/Main
Auto-merging app.py
Merge made by the 'ort' strategy.
 app.py | 6 +++---
 1 file changed, 3 insertions(+), 3 deletions(-)

(venv) C:\GitPractice>git push origin Main
Enumerating objects: 10, done.
Counting objects: 100% (10/10), done.
Delta compression using up to 12 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 687 bytes | 343.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
To https://github.com/anuraggit6212/PracticeGit.git
   243ad76..eaddcc9  Main -> Main

(venv) C:\GitPractice>git add.
git: 'add.' is not a git command. See 'git --help'.

The most similar command is
        add

(venv) C:\GitPractice>git add .

(venv) C:\GitPractice>git status
On branch Main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   app.py


(venv) C:\GitPractice>git commit -m "Updated sub again in app"
[Main c6df560] Updated sub again in app
 1 file changed, 2 insertions(+), 2 deletions(-)

(venv) C:\GitPractice>git push origin Main
To https://github.com/anuraggit6212/PracticeGit.git
 ! [rejected]        Main -> Main (fetch first)
error: failed to push some refs to 'https://github.com/anuraggit6212/PracticeGit.git'
hint: Updates were rejected because the remote contains work that you do not      
hint: have locally. This is usually caused by another repository pushing to       
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.        

(venv) C:\GitPractice>git pull origin Main
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 971 bytes | 28.00 KiB/s, done.
From https://github.com/anuraggit6212/PracticeGit
 * branch            Main       -> FETCH_HEAD
   eaddcc9..3a63709  Main       -> origin/Main
Auto-merging app.py
CONFLICT (content): Merge conflict in app.py
Automatic merge failed; fix conflicts and then commit the result.

(venv) C:\GitPractice>git pull origin Main
error: Pulling is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: Exiting because of an unresolved conflict.

(venv) C:\GitPractice>git add .

(venv) C:\GitPractice>git status
On branch Main
All conflicts fixed but you are still merging.
  (use "git commit" to conclude merge)

Changes to be committed:
        modified:   app.py


(venv) C:\GitPractice>git commit -m "Resolved merge conflicts"
[Main 7fed7f9] Resolved merge conflicts

(venv) C:\GitPractice>git push origin Main
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 12 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 530 bytes | 176.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/anuraggit6212/PracticeGit.git
   3a63709..7fed7f9  Main -> Main

(venv) C:\GitPractice>git log
commit 7fed7f9e3903d954bfd53729466fec060875ba93 (HEAD -> Main, origin/Main)
Merge: c6df560 3a63709
Author: Anurag Mahalpure <anuragmahalpure@gmail.com>
Date:   Sat Oct 4 21:29:43 2025 +0530

    Resolved merge conflicts
:
commit 7fed7f9e3903d954bfd53729466fec060875ba93 (HEAD -> Main, origin/Main)       
Merge: c6df560 3a63709
Author: Anurag Mahalpure <anuragmahalpure@gmail.com>
Date:   Sat Oct 4 21:29:43 2025 +0530

    Resolved merge conflicts
:
commit 7fed7f9e3903d954bfd53729466fec060875ba93 (HEAD -> Main, origin/Main)       
Merge: c6df560 3a63709
Author: Anurag Mahalpure <anuragmahalpure@gmail.com>
Date:   Sat Oct 4 21:29:43 2025 +0530

    Resolved merge conflicts
: