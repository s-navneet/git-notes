first we have to make a repo on github
and the we make a directory on local machine
then we clone or remote


STARTING

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

------------REBASEING-----

git checkout dev
git pull origin dev
git checkout branch-name
git rebase dev
RESOLVE CONFLICTS
git add .
git push origin branch-name --force



--------CYPRESSS-WSL--------


after install cypress perform these steps to setup cypress with wsl in window
1. sudo apt update
2. sudo apt upgrade
3. sudo apt install libgtk-3-dev libnotify-dev libgconf-2-4 libnss3 libxss1 libasound2
4. export DISPLAY=$(cat /etc/resolv.conf | grep nameserver | awk '{print $2; exit;}'):0.0
5. sudo /etc/init.d/dbus start &> /dev/null
6. sudo visudo -f /etc/sudoers.d/dbus  => file open enter name here (<your_username> ALL = (root) NOPASSWD: /etc/init.d/dbus) save it

after cypress version update and for open cypress

1. open x-server 
2. then open ubuntu
3. set display (export DISPLAY=$(cat /etc/resolv.conf | grep nameserver | awk '{print $2; exit;}'):0.0)
4. npx cypress verify
5. npx cypress open

------------npm regestry-----
npm login --registry=https://npm.pkg.github.com --scope=@geospoc
username: <your github username>
password: <your github personal access token>
