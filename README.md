#Myapp
This is my App
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   app.js

no changes added to commit (use "git add" and/or "git commit -a")

Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ git add .

Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ git commit -m 'changed app.js'
[master 72f56ae] changed app.js
 1 file changed, 1 insertion(+)

Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ clear

Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ touch .gitignore

Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ touch log.text

Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ git add .

Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   .gitignore
        new file:   log.text


Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   .gitignore
        new file:   log.text

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        deleted:    log.text


Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ git add .

Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   .gitignore


Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ git add .

Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   .gitignore
        new file:   dir1/app1.js


Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   .gitignore
        new file:   dir1/app1.js

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   .gitignore


Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ git add .

Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   .gitignore
        new file:   dir1/app1.js


Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ git branch
* master

Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ git branche login
git: 'branche' is not a git command. See 'git --help'.

The most similar command is
        branch

Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ git branch login

Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   .gitignore
        new file:   dir1/app1.js


Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ git commit -m 'an other change'
[master 8fc1ea5] an other change
 2 files changed, 4 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 dir1/app1.js

Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ git checkout login
Switched to branch 'login'

Tarik1@Tarik MINGW64 ~/Desktop/gittest (login)
$ toouch login.html
bash: toouch: command not found

Tarik1@Tarik MINGW64 ~/Desktop/gittest (login)
$ touch login.html

Tarik1@Tarik MINGW64 ~/Desktop/gittest (login)
$ git status
On branch login
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   index.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        dir2/
        log.txt
        login.html

no changes added to commit (use "git add" and/or "git commit -a")

Tarik1@Tarik MINGW64 ~/Desktop/gittest (login)
$ git add .

Tarik1@Tarik MINGW64 ~/Desktop/gittest (login)
$ git commit -m 'after login'
[login 13c9f17] after login
 4 files changed, 4 insertions(+)
 create mode 100644 dir2/app2.js
 create mode 100644 log.txt
 create mode 100644 login.html

Tarik1@Tarik MINGW64 ~/Desktop/gittest (login)
$ git status
On branch login
nothing to commit, working tree clean

Tarik1@Tarik MINGW64 ~/Desktop/gittest (login)
$ git checkout master
Switched to branch 'master'

Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ git checkout login
Switched to branch 'login'

Tarik1@Tarik MINGW64 ~/Desktop/gittest (login)
$ git status
On branch login
nothing to commit, working tree clean

Tarik1@Tarik MINGW64 ~/Desktop/gittest (login)
$ git checkout master
Switched to branch 'master'

Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ gitmerge login
bash: gitmerge: command not found

Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ git merge login
Merge made by the 'recursive' strategy.
 dir2/app2.js | 1 +
 index.html   | 1 +
 log.txt      | 1 +
 login.html   | 1 +
 4 files changed, 4 insertions(+)
 create mode 100644 dir2/app2.js
 create mode 100644 log.txt
 create mode 100644 login.html

Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ git remote

Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ git remote add origin https://github.com/Kastarik/gitapp.git

Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ git remote
origin

Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ git push -u origin master
Counting objects: 21, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (12/12), done.
Writing objects: 100% (21/21), 1.72 KiB | 126.00 KiB/s, done.
Total 21 (delta 4), reused 0 (delta 0)
remote: Resolving deltas: 100% (4/4), done.
To https://github.com/Kastarik/gitapp.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.

Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ touch README.md

Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ git add .

Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ git commit -m 'Added readme'
[master 03a24dd] Added readme
 1 file changed, 2 insertions(+)
 create mode 100644 README.md

Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ git push
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 299 bytes | 149.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Kastarik/gitapp.git
   70a82aa..03a24dd  master -> master

Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ git remote
origin

Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ remote
bash: remote: command not found

Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$ git remote
origin

Tarik1@Tarik MINGW64 ~/Desktop/gittest (master)
$
