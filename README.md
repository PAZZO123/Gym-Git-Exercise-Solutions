# Gym-Git-Exercise-Solutions
## Bundle 1
### Exercise 1

``` bash

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym
$ mkdir Git_Exercises

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym
$ cd git_exercises

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises
$ git init
Initialized empty Git repository in C:/Users/USER/Desktop/TheGym/Git_Exercises/.git/

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (main)
$ git status
On branch main

No commits yet

nothing to commit (create/copy files and use "git add" to track)

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (main)
$ echo hello>myfile.js

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (main)
$ ls
myfile.js

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (main)
$ git branch -M master

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (master)
$ git add myfile.js
warning: in the working copy of 'myfile.js', LF will be replaced by CRLF the next time Git touches it

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   myfile.js
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (master)
$ git commit -m "Creating First File"
[master (root-commit) 0d24f27] Creating First File
 1 file changed, 1 insertion(+)
 create mode 100644 myfile.js
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (master)
$ git remote add origin https://github.com/PAZZO123/Git-Exercises.git
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (master)
$ git push -u origin master
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 232 bytes | 232.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/PAZZO123/Git-Exercises.git
 * [new branch]      master -> master
branch 'master' set up to track 'origin/master'.
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (master)
$ git branch dev

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (master)
$ git switch dev
Switched to branch 'dev'

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (dev)
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (dev)
$ git push --all
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/PAZZO123/Git-Exercises/pull/new/dev
remote:
To https://github.com/PAZZO123/Git-Exercises.git
 * [new branch]      dev -> dev

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (dev)
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (dev)
$ git checkout -b test
Switched to a new branch 'test'

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (test)
$ git push -u origin test
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/PAZZO123/Git-Exercises/pull/new/test
remote:
To https://github.com/PAZZO123/Git-Exercises.git
 * [new branch]      test -> test
branch 'test' set up to track 'origin/test'.

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (test)
$

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (test)
$ git switch dev
Switched to branch 'dev'

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (dev)
$ git branch -d test
Deleted branch test (was 0d24f27).

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (dev)
$ git branch
* dev
  master

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (dev)
```
