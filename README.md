# Gym-Git-Exercise-Solutions

## Bundle 1

### Excercise 1

``` bash
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        try.js

nothing added to commit but untracked files present (use "git add" to track)
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git add .
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   try.js

brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git commit -m "hello world"
[main aa117f3] hello world
 1 file changed, 1 insertion(+)
 create mode 100644 try.js
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 305 bytes | 305.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/BrendaGilisho/Ojemba_X_the_Gym.git
   298e483..aa117f3  main -> main
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git checkout -b dev
Switched to a new branch 'dev'
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git checkout -b test
Switched to a new branch 'test'
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git checkout dev
Switched to branch 'dev'
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git branch -d test
Deleted branch test (was aa117f3).
```
### Excercise 2

``` bash
brendagilisho@brenda:~/coding_projects/Gym-Git-Exercise-Solutions$ git stash save "home"
No local changes to save
brendagilisho@brenda:~/coding_projects/Gym-Git-Exercise-Solutions$ git stash save "home"
No local changes to save
brendagilisho@brenda:~/coding_projects/Gym-Git-Exercise-Solutions$ git add .
brendagilisho@brenda:~/coding_projects/Gym-Git-Exercise-Solutions$ git stash save "home"
Saved working directory and index state On main: home
brendagilisho@brenda:~/coding_projects/Gym-Git-Exercise-Solutions$ ^C
brendagilisho@brenda:~/coding_projects/Gym-Git-Exercise-Solutions$ git add .
brendagilisho@brenda:~/coding_projects/Gym-Git-Exercise-Solutions$ git stash save "about"
Saved working directory and index state On main: about
brendagilisho@brenda:~/coding_projects/Gym-Git-Exercise-Solutions$ ^C
brendagilisho@brenda:~/coding_projects/Gym-Git-Exercise-Solutions$ git add .
brendagilisho@brenda:~/coding_projects/Gym-Git-Exercise-Solutions$ git stash save "team"
Saved working directory and index state On main: team
brendagilisho@brenda:~/coding_projects/Gym-Git-Exercise-Solutions$ git stash list
stash@{0}: On main: team
stash@{1}: On main: about
stash@{2}: On main: home
```
## Bundle 2

### Excercise 1

```bash
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git add .
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git commit -m "pullreq & merge"
[ft/bundle-2 b3f8d8c] pullreq & merge
 3 files changed, 47 insertions(+), 1 deletion(-)
 create mode 100644 grid/task3-1.html
 create mode 100644 services.html
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git push
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git push --set-upstream origin ft/bundle-2
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 8 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 1.02 KiB | 349.00 KiB/s, done.
Total 6 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/BrendaGilisho/Ojemba_X_the_Gym/pull/new/ft/bundle-2
remote: 
To https://github.com/BrendaGilisho/Ojemba_X_the_Gym.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.
```
### Excercise 2

```bash
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git pull
Already up to date.
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git add .
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git commit -m 'service-redesign'
[ft/service-redesign 5210e53] service-redesign
 1 file changed, 16 insertions(+)
 create mode 100644 services.html
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git push --set-upstream origin ft/service-redesign
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 609 bytes | 609.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/BrendaGilisho/Ojemba_X_the_Gym/pull/new/ft/service-redesign
remote: 
To https://github.com/BrendaGilisho/Ojemba_X_the_Gym.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git add .
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git commit -m 'update'
[main c38c256] update
 1 file changed, 17 insertions(+)
 create mode 100644 services.html
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 545 bytes | 272.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/BrendaGilisho/Ojemba_X_the_Gym.git
   014ddc6..c38c256  main -> main
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git diff ft/service-redesign..main
diff --git a/services.html b/services.html
index 02b330c..daba37a 100644
--- a/services.html
+++ b/services.html
@@ -8,8 +8,9 @@
 </head>
 <body>
     <div>
-        <h1>Pull Requests</h1>
-        <p>Here’s a list of pull requests you can review. If you’re not sure where to start, try the ones with the most recent activity.</p>
+        <h1 class="test-h1">Pull Requests</h1>
+        <p class="test-p">Git activities</p>
+        <div></div>
     </div>
     
 </body>
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git merge
Already up to date.
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ 
 *  History restored 

brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git fetch
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git pull
Already up to date.
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git status
On branch ft/service-redesign
Your branch is up to date with 'origin/ft/service-redesign'.

nothing to commit, working tree clean
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git merge main
Auto-merging services.html
CONFLICT (add/add): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git add .
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git commit
[ft/service-redesign b4041d6] Merge branch 'main' into ft/service-redesign
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git push
Enumerating objects: 1, done.
Counting objects: 100% (1/1), done.
Writing objects: 100% (1/1), 243 bytes | 243.00 KiB/s, done.
Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/BrendaGilisho/Ojemba_X_the_Gym.git
   5210e53..b4041d6  ft/service-redesign -> ft/service-redesign
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ 
```
## Bundle 3

### Excercise 1

``` bash
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git add .
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git commit -m 'team'
[ft/team-page 0afb9e5] team
 1 file changed, 12 insertions(+)
 create mode 100644 team.html
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git push --set-upstream origin ft/team-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 445 bytes | 445.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/BrendaGilisho/Ojemba_X_the_Gym/pull/new/ft/team-page
remote: 
To https://github.com/BrendaGilisho/Ojemba_X_the_Gym.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git  checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git checkout ft/team-page
Already on 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.
brendagilisho@brenda:~/coding_projects/Ojemba_X_the_Gym$ git log
commit 0afb9e549be25f3d4b26221f6aa1ebcd6c921bcc (HEAD -> ft/team-page, origin/ft/team-page)
Author: BrendaGilisho <b.gilisho@alustudent.com>
Date:   Tue May 23 10:08:52 2023 +0200

    team

commit b4041d62458da2a3149c34dd678ab77fe29c8207 (origin/ft/service-redesign, ft/service-redesign)
Merge: 5210e53 c38c256
Author: BrendaGilisho <b.gilisho@alustudent.com>
Date:   Tue May 23 08:00:10 2023 +0200

    Merge branch 'main' into ft/service-redesign

commit c38c2560e7e4638f0ed6b60e50c4666e38d3d794 (origin/main, origin/HEAD, main, ft/contact-page)
Author: BrendaGilisho <b.gilisho@alustudent.com>
Date:   Tue May 23 05:37:12 2023 +0200

    update

commit 5210e53048c0445bd0b0517f2734c7c23108122a
Author: BrendaGilisho <b.gilisho@alustudent.com>
Date:   Tue May 23 05:23:06 2023 +0200

    service-redesign

commit 014ddc61a5c8fd468fe433f9dbd2cbe46c0ed861
Author: BrendaGilisho <b.gilisho@alustudent.com>
Date:   Wed May 17 23:43:11 2023 +0200

    grid

commit b4024c2a1656bc4307a023fc940ed717e5252216
Author: BrendaGilisho <b.gilisho@alustudent.com>
Date:   Wed May 17 23:04:15 2023 +0200

    grid

commit aa117f35f3a98b29702ad18facfdd04ae12499ca (origin/dev, dev)
Author: BrendaGilisho <b.gilisho@alustudent.com>
Date:   Sun May 14 17:31:04 2023 +0200

    hello world

commit 298e483a1b824dc98831556a29b75b50ddf73c76
Author: Brenda Gilisho <57228014+BrendaGilisho@users.noreply.github.com>
Date:   Tue May 9 05:55:58 2023 +0200

    Initial commit
```
