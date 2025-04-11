<!-- initialize the git repo -->
Aman@LAPTOP-NTVJKTQ8 MINGW64 ~/OneDrive/Desktop/devops-project (master)
$ git init
Initialized empty Git repository in C:/Users/Aman/OneDrive/Desktop/devops-prot/.git
 
% Link your local repo to GitHub:
Aman@LAPTOP-NTVJKTQ8 MINGW64 ~/OneDrive/Desktop/devops-project (main)
$ git remote add origin https://github.com/amangoswami177/devops-project.git

<!-- create file by using touch command in git bash -->
Aman@LAPTOP-NTVJKTQ8 MINGW64 ~/OneDrive/Desktop/devops-project (main)
$ touch index.html

% changes added to the git staging area
Aman@LAPTOP-NTVJKTQ8 MINGW64 ~/OneDrive/Desktop/devops-project (main)
$ git add .

<!-- commited the changes -->
Aman@LAPTOP-NTVJKTQ8 MINGW64 ~/OneDrive/Desktop/devops-project (main)
$ git commit -m "first commit"
[main (root-commit) 782787a] first commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 index.html

% Before pusing cahnges to github pull the changes to git bash
Aman@LAPTOP-NTVJKTQ8 MINGW64 ~/OneDrive/Desktop/devops-project (main)
$ git pull origin main --rebase
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 871 bytes | 79.00 KiB/s, done.
From https://github.com/amangoswami177/devops-project
 * branch            main       -> FETCH_HEAD
 * [new branch]      main       -> origin/main
Successfully rebased and updated refs/heads/main.

<!-- chnages pushed to github -->
Aman@LAPTOP-NTVJKTQ8 MINGW64 ~/OneDrive/Desktop/devops-project (main)
$ git push -u origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 276 bytes | 276.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/amangoswami177/devops-project.git
   b211854..5d793d0  main -> main
branch 'main' set up to track 'origin/main'.

% created branches and switch to that branch
Aman@LAPTOP-NTVJKTQ8 MINGW64 ~/OneDrive/Desktop/devops-project (main)
$ git checkout -b dev
Switched to a new branch 'dev'

Aman@LAPTOP-NTVJKTQ8 MINGW64 ~/OneDrive/Desktop/devops-project (dev)
$ git checkout -b feature
Switched to a new branch 'feature'

% Changes pushed to the branches
Aman@LAPTOP-NTVJKTQ8 MINGW64 ~/OneDrive/Desktop/devops-project (main)
$ git push -u origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/amangoswami177/devops-project/pull/new/dev
remote:
To https://github.com/amangoswami177/devops-project.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.

Aman@LAPTOP-NTVJKTQ8 MINGW64 ~/OneDrive/Desktop/devops-project (feature)
$ git push -u origin feature
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'feature' on GitHub by visiting:
remote:      https://github.com/amangoswami177/devops-project/pull/new/feature
remote:
To https://github.com/amangoswami177/devops-project.git
 * [new branch]      feature -> feature
branch 'feature' set up to track 'origin/feature'.

% Once you have a stable version on main, add a version tag and pusdhed to main branch

Aman@LAPTOP-NTVJKTQ8 MINGW64 ~/OneDrive/Desktop/devops-project (main)
$ git tag -a v1.0 -m "First stable release"

Aman@LAPTOP-NTVJKTQ8 MINGW64 ~/OneDrive/Desktop/devops-project (main)
$ git push origin v1.0
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 518 bytes | 518.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/amangoswami177/devops-project.git
 * [new tag]         v1.0 -> v1.0




