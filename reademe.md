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
