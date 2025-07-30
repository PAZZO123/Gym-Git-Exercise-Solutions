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
$ git branch -M main

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (main)
$ git add myfile.js
warning: in the working copy of 'myfile.js', LF will be replaced by CRLF the next time Git touches it

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   myfile.js
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (main)
$ git commit -m "Creating First File"
[main (root-commit) 0d24f27] Creating First File
 1 file changed, 1 insertion(+)
 create mode 100644 myfile.js
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (main)
$ git remote add origin https://github.com/PAZZO123/Git-Exercises.git
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (main)
$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 232 bytes | 232.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/PAZZO123/Git-Exercises.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (main)
$ git branch dev

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (main)
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
  main

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

## Bundle 2
### Exercise 1


```bash
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (ft/bundle-2)
$ git status
On branch ft/bundle-2
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Services.html

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (ft/bundle-2)
$ git add .
warning: in the working copy of 'Services.html', LF will be replaced by CRLF the next time Git touches it

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (ft/bundle-2)
$ git stash
Saved working directory and index state WIP on ft/bundle-2: c6f2d46 Just a Test foor team

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (ft/bundle-2)
$ git stash pop
On branch ft/bundle-2
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   Services.html

Dropped refs/stash@{0} (ba34c0ae60e0d5a33562ae339c9c4126bb827c58)

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (ft/bundle-2)
$ git commit -m "Adding Services"
[ft/bundle-2 ccb7786] Adding Services
 1 file changed, 11 insertions(+)
 create mode 100644 Services.html

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (ft/bundle-2)
$ git push -u origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 446 bytes | 446.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/PAZZO123/Git-Exercises/pull/new/ft/bundle-2
remote:
To https://github.com/PAZZO123/Git-Exercises.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.
```

### Exercise 2

```bash

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (main)
$ git fetch
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (1/1), 958 bytes | 239.00 KiB/s, done.
From https://github.com/PAZZO123/Git-Exercises
   0d24f27..065129c  main     -> origin/main

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (main)
$ git merge
Updating 0d24f27..065129c
Fast-forward
 Services.html | 11 +++++++++++
 about.html    |  1 +
 home.html     | 11 +++++++++++
 team.html     |  1 +
 4 files changed, 24 insertions(+)
 create mode 100644 Services.html
 create mode 100644 about.html
 create mode 100644 home.html
 create mode 100644 team.html
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/main'.
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (ft/service-redesign)
$ git  status
On branch ft/service-redesign
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   Services.html
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (ft/service-redesign)
$ git add .

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (ft/service-redesign)
$ git commit -m 'Changed Services'
[ft/service-redesign 8d80292] Changed Services
 1 files changed, 7 insertions(+), 1 deletions(-)
 USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (ft/service-redesign)
$ git push -u origin ft/service-redesign
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 12 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 669 bytes | 669.00 KiB/s, done.
Total 6 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), completed with 1 local objects.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/PAZZO123/Git-Exercises/pull/new/ft/service-redesign
remote:
To https://github.com/PAZZO123/Git-Exercises.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (main)
$
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (main)
$ git add .

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (main)
$ git commit -m 'Changed Services In main'
[main 8d80292] Changed Services
 1 files changed, 7 insertions(+), 1 deletions(-)
 USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/git_exercises (main)
$ git push -u origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 669 bytes | 669.00 KiB/s, done.
Total 6 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), completed with 1 local objects.
remote:
remote: Create a pull request for 'main' on GitHub by visiting:
remote:      https://github.com/PAZZO123/Git-Exercises/pull/new/main
remote:
To https://github.com/PAZZO123/Git-Exercises.git
 * [new branch]      main -> main
branch 'main' set up to track 'main'.

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/service-redesign)
$ git merge main
Auto-merging Services.html
CONFLICT (content): Merge conflict in Services.html
Automatic merge failed; fix conflicts and then commit the result.
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/service-redesign|MERGING)
$ git diff
diff --cc Services.html
index ef2e309,7bd1f7f..0000000
--- a/Services.html
+++ b/Services.html
@@@ -6,14 -6,11 +6,18 @@@
      <title>Document</title>
  </head>
  <body>
++<<<<<<< HEAD
 +    <h1>Our OLd Services</h1>
++=======
+     <h1>Our  Main Services</h1>
++>>>>>>> main
      <ul>
 -        <li>one</li>
 -        <li>two</li>
 -        <li>three</li>
 +        <li>First</li>
 +        <li>
 +            second
 +        </li>
 +        <li>Third</li>
 +
      </ul>
  </body>
  </html>

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/service-redesign|MERGING

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/service-redesign|MERGING)
$
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/service-redesign|MERGING)
$ git add .

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/service-redesign|MERGING)
$ git commit -m 'Resolving conflict'
[ft/service-redesign 6112cff] Resolving conflict

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/service-redesign)
$ git push -u origin ft/service-redesign
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 365 bytes | 365.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/PAZZO123/Git-Exercises.git
   8d80292..6112cff  ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.

```
## Bundle 3
### Exercise 1

```bash
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (main)
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/team-page)
$ touch team.htm

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/team-page)
$ git add team.htm
warning: in the working copy of 'team.htm', LF will be replaced by CRLF the next time Git touches it

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/team-page)
$ git stash
Saved working directory and index state WIP on ft/team-page: da9206d Second change in main

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/team-page)
$ git stash pop
On branch ft/team-page
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.htm

Dropped refs/stash@{0} (548df1e2ba386f724802b846d6a3dc9d01d8723a)

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/team-page)
$ git commit -m "Add Team.htm to Team-page"
[ft/team-page dc05025] Add Team.htm to Team-page
 1 file changed, 11 insertions(+)
 create mode 100644 team.htm
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/team-page)
$ git push -u origin ft/team-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 435 bytes | 435.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/PAZZO123/Git-Exercises/pull/new/ft/team-page
remote:
To https://github.com/PAZZO123/Git-Exercises.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/team-page)
$ git log
commit dc050258e07d55c2e73fb35390aeea2a0d11f459 (HEAD -> ft/team-page, origin/ft/team-page)
Author: PAZZO123 <smbabazipatrick@gmail.com>
Date:   Wed Jul 30 17:10:38 2025 +0200

    Add Team.htm to Team-page

commit da9206dc1162792e0fe8949c80838666c7684056 (origin/main, main, ft/contact-page)
Author: PAZZO123 <smbabazipatrick@gmail.com>
Date:   Wed Jul 30 10:41:18 2025 +0200

    Second change in main

commit a907672e6ff8d0ced027b3ef811d3c81231d844a
Author: PAZZO123 <smbabazipatrick@gmail.com>
Date:   Tue Jul 29 20:58:11 2025 +0200

    Second change in master branch

commit 065129c8711217d26eead12297c6fd36d749ab6f
Merge: 0d24f27 ccb7786
Author: Straton patrick Mbabazi <154052094+PAZZO123@users.noreply.github.com>
Date:   Tue Jul 29 20:27:12 2025 +0200

    Merge pull request #1 from PAZZO123/ft/bundle-2

    Ft/bundle 2-Added another files home.hml,about.html,team.html and services.html

commit ccb77862f8278dc34de614316d9a2b4d150389c6 (origin/ft/bundle-2, ft/bundle-2)
Author: PAZZO123 <smbabazipatrick@gmail.com>
Date:   Tue Jul 29 19:23:07 2025 +0200

    Adding Services

commit c6f2d46b6e3b281dd6171a69ab645f22b8dcbfed (origin/dev, dev)
Author: PAZZO123 <smbabazipatrick@gmail.com>
Date:   Tue Jul 29 18:16:18 2025 +0200

    Just a Test foor team

commit d0491b892b3e774dbd88b5ca9286730dda66f3a1
Author: PAZZO123 <smbabazipatrick@gmail.com>
Date:   Tue Jul 29 18:08:13 2025 +0200

    Just a Test

commit 0d24f2793117f0a6586c85d565b54581873d3693 (origin/test)
Author: PAZZO123 <smbabazipatrick@gmail.com>
Date:   Tue Jul 29 17:02:20 2025 +0200

    Creating First File
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/contact-page)
$ git cherry-pick  dc050258e07d55c2e73fb35390aeea2a0d11f459
[ft/contact-page 7b7bbba] Add Team.htm to Team-page
 Date: Wed Jul 30 17:10:38 2025 +0200
 1 file changed, 11 insertions(+)
 create mode 100644 team.htm

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/contact-page)
$ touch contact.html

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/contact-page)
$ git add contact.html
warning: in the working copy of 'contact.html', LF will be replaced by CRLF the next time Git touches it

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/contact-page)
$ git stash
Saved working directory and index state WIP on ft/contact-page: 7b7bbba Add Team.htm to Team-page

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/contact-page)
$ git stash pop
On branch ft/contact-page
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   contact.html

Dropped refs/stash@{0} (f7848b3ba83d29e6f07d290e69cd22bf79edb066)

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/contact-page)
$ git commit -m "Add Contact Page File"
[ft/contact-page 07c9c2f] Add Contact Page File
 1 file changed, 11 insertions(+)
 create mode 100644 contact.html

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/contact-page)
$ git push -u origin ft/contact-page
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 12 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 716 bytes | 716.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/PAZZO123/Git-Exercises/pull/new/ft/contact-page
remote:
To https://github.com/PAZZO123/Git-Exercises.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/contact-page)
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/faq-page)
$ touch faq.html

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/faq-page)
$ git status
On branch ft/faq-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        faq.html

nothing added to commit but untracked files present (use "git add" to track)

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/faq-page)
$ git add faq.html
warning: in the working copy of 'faq.html', LF will be replaced by CRLF the next time Git touches it

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/faq-page)
$ git commit -m "Add Faq Page"
[ft/faq-page fddf2ec] Add Faq Page
 1 file changed, 11 insertions(+)
 create mode 100644 faq.html

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/faq-page)
$ git push -u origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 433 bytes | 433.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/PAZZO123/Git-Exercises/pull/new/ft/faq-page
remote:
To https://github.com/PAZZO123/Git-Exercises.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/faq-page)
$ git revert  dc050258e07d55c2e73fb35390aeea2a0d11f459
[ft/faq-page aa2b883] Revert "Add Team.htm to Team-page"
 1 file changed, 11 deletions(-)
 delete mode 100644 team.htm

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/faq-page)
$ git log
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/faq-page)
$ git push -u origin ft/faq-page
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 295 bytes | 295.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/PAZZO123/Git-Exercises.git
   fddf2ec..aa2b883  ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.

```
### Exercise 2
```bash
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/faq-page)
$ git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/home-page-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is based on 'origin/master', but the upstream is gone.
  (use "git branch --unset-upstream" to fixup)

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (main)
$ git add .


USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (main)
$ git commit -m "feat: Add Some Changes"
[main 88f86ad] feat: Add Some Changes
 1 file changed, 1 insertion(+)
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (main)
$ git push -u origin main
To https://github.com/PAZZO123/Git-Exercises.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/PAZZO123/Git-Exercises.git'
hint: Updates were rejected because the remote contains work that you do not
hint: have locally. This is usually caused by another repository pushing to
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/home-page-redesign)
$ git rebase main
Successfully rebased and updated refs/heads/ft/home-page-redesign.

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/home-page-redesign)
$ git log
USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/home-page-redesign)
$ git add .

USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/home-page-redesign)
$ git commit -m "Feat: After rebase"
[ft/home-page-redesign 40537f9] Feat: After rebase
 1 file changed, 3 insertions(+)
 USER@LAPTOP-MGOER4DS MINGW64 ~/desktop/thegym/Git_Exercises (ft/home-page-redesign)
$ git push -u origin ft/home-page-redesign
Enumerating objects: 19, done.
Counting objects: 100% (19/19), done.
Delta compression using up to 12 threads
Compressing objects: 100% (17/17), done.
Writing objects: 100% (17/17), 1.85 KiB | 474.00 KiB/s, done.
Total 17 (delta 9), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (9/9), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/PAZZO123/Git-Exercises/pull/new/ft/home-page-redesign
remote:
To https://github.com/PAZZO123/Git-Exercises.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
branch 'ft/home-page-redesign' set up to track 'origin/ft/home-page-redesign'.

```

