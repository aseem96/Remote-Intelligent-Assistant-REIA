README

Upload all versions of the project report, present and future, here.

SETUP

1. git config --global user.name "USER_NAME"
2. git config --global user.email "EMAIL_ID"

PULL CODE

1. cd BE-Project
2. HTTPS: git pull https://gitlab.com/BE-Project/REIA.git master
3. SSH  : git pull git@gitlab.com:BE-Project/REIA.git

Refer https://docs.gitlab.com/ee/gitlab-basics/create-your-ssh-keys.html to setup ssh key

Choose either of 2 or 3.

DELIVER CODE

1. cd BE-Project
2. git init
3. git remote add origin git@gitlab.com:BE-Project/REIA.git
4. git add .
5. git commit -m "COMMIT MESSAGE"
6. git push -u origin master

INSTALL DEPENDENCIES

pip install -r requirements.txt
# Remote-Intelligent-Assistant-REIA
