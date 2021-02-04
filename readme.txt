first we have to make a repo on github
and the we make a directory on local machine
then we clone or remote


starting

git config --global user.name "your name"
git config --global user.email "your email(github email acc)"

git clone "copy thr url of repo"  -> copy the entire file and paste into ur local

git remote add origin "copy the url of repo" -> make a remote connection

git init

git status

git add filename

git commit

git push origin master -f

if you want to pull

git pull origin master

how to remove remote

git remote -v

git remote rm origin

how to add branch

git checkout -b branchName

rebasing-----

git checkout dev
git pull origin dev
git checkout branch-name
git rebase dev
RESOLVE CONFLICTS
git add .
git push origin branch-name --force
