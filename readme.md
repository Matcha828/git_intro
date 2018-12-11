#INSTALL GIT
#1、检查ssh keys是否存在
* $ ls -al ~/.ssh

#2、生成ssh key
* $ssh-keygen -t rsa -b 4096 -C "your_email@example.com"

#3、将ssh key添加到ssh-agent
* eval $(ssh-agent -s)

#4 将ssh key添加到ssh-agent
* $ssh-add ~/.ssh/id_rsa

#5 copy your ssh key
* cat ~/.ssh/id_rsa.pub

#6 Add ssh key to Github account and run
* $ git clone git@github.com:Matcha828/git_intro.git

* git remote add origin git@github.com:Matcha828/git_intro.git

* git push origin master

/////////////////////////
* git revert --no-commit daf1rqr1rn1n21j..HEAD
* git commit -m """

#USE GIT
* 1. git init
* 2. git status

## add files
* 3. git add <file>
* 3a. git add *.<type> (add certain type)
* 3b. git add -A (add all files and directory you are in)

* 4. git commit -m "text"

* 5. git log (check records)
* 6. git checkout (check previous repo) 

## revert files to previous version
* 7. git revert --no-commit daf1rqr1rn1n21j..HEAD
* 7a. git commit -m """

## remove files from stages
* 8 git reset HEAD <file> (remove files from stage)

## ignore files
* 9. touch .gitignore
* 9a. open gitignore file and add the file name we want to ignore
* 9b. git add -A and git commit -m "add gitignore"




