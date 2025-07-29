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

### Exercise2

```bash
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (dev)
$ echo htm>home.html

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (dev)
$ git add home.html
warning: in the working copy of 'home.html', LF will be replaced by CRLF the next time Git touches it

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (dev)
$ git stash
Saved working directory and index state WIP on dev: 0d24f27 Creating First File
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (dev)
$ echo about >about.html
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (dev)
$ git add about.html
warning: in the working copy of 'about.html', LF will be replaced by CRLF the next time Git touches it

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (dev)
$ git stash
Saved working directory and index state WIP on dev: 0d24f27 Creating First File

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (dev)
$ git stash list
stash@{0}: WIP on dev: 0d24f27 Creating First File
stash@{1}: WIP on dev: 0d24f27 Creating First File

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (dev)
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (dev)
$ echo Team>team.html

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (dev)
$ git add team.html
warning: in the working copy of 'team.html', LF will be replaced by CRLF the next time Git touches it

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (dev)
$ git stash
Saved working directory and index state WIP on dev: 0d24f27 Creating First File

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (dev)
$ git stash list
stash@{0}: WIP on dev: 0d24f27 Creating First File
stash@{1}: WIP on dev: 0d24f27 Creating First File
stash@{2}: WIP on dev: 0d24f27 Creating First File

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (dev)
$ git stash pop stash@{1}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (b8a70fb8d0d1ad9cb3d1d6f2267b51a8fac66aaa)

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (dev)
$ git stash list
stash@{0}: WIP on dev: 0d24f27 Creating First File
stash@{1}: WIP on dev: 0d24f27 Creating First File

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (dev)
$ git stash pop stash@{1}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (b79cf809e5dfedcf79657e45c195a8aa6beea218)
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (dev)
$ git commit -m "Just a Test"
[dev d0491b8] Just a Test
 2 files changed, 12 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (dev)
$ git push -u origin dev
fatal: unable to access 'https://github.com/PAZZO123/Git-Exercises.git/': Recv failure: Connection was reset

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (dev)
$ git push -u origin dev
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 482 bytes | 160.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/PAZZO123/Git-Exercises.git
   0d24f27..d0491b8  dev -> dev
branch 'dev' set up to track 'origin/dev'.

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (dev)
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (dev)
$ git stash pop stash@{0}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped stash@{0} (d2768e2a6e7b0c7b47b2541f10aff1c37d427511)

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (dev)
$ git commit -m "Just a Test foor team"
[dev c6f2d46] Just a Test foor team
 1 file changed, 1 insertion(+)
 create mode 100644 team.html
 USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (dev)
$ git reset --hard
HEAD is now at c6f2d46 Just a Test foor team



```
