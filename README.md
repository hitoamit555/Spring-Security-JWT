# Spring-Security-JWT
SpringBoot Security with JWT

**Git Commands and step to create new repo first time**

1.Goto git browser and create repo with same name as local created. And follow cmd below.

2.Goto local and follow below cmd

  git init
  
  git add .
  
  git commit -m "Initial commit"
  
  git remote add origin youruser@yourserver.com:/path/to/my_project.git
  
  git push -u origin master
  
If User not added into local pc(Adding new users)

  git config --global user.email "you@examole.com"
  git config --global user.name "Your name"
  git push -u origin master
  Then popup window will open asking for git username and passwword

Check list of user if added duplicate and remove/replace

  git config --list
  git config --global --replace-all user.email "you@examole.co"
  git config --global --add user.email "you@examole.co"

  
  

**Remove/add user into computer for Windows**

Control panel > useraccount >credential >Generic credential
Next Remove the github key
and again add user into cmd 
  

########################

mkdir my_project
cd my_project
touch .gitignore
git init
git add .
git commit -m "Initial commit"
git remote add origin youruser@yourserver.com:/path/to/my_project.git
git push origin master

##########################


**Url :localhost:8080 **
Input request
```json
{
"name": "username",
"email": "email"
}
```
   
