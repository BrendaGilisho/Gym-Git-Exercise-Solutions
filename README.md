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
