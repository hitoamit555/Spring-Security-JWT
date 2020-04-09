# Spring-Security-JWT
SpringBoot Security with JWT

**Git Commands and step to create new repo first time**

1.Goto git browser and create repo with same name as local created. And copy url of you Repo and follow cmd below.

2.Goto local PC and follow below cmd
  ~~~ 
  cd my_project
  git init
  git add .
  git commit -m "Initial commit"
  git remote add origin youruser@yourserver.com:/path/to/my_project.git
  git push -u origin master
  ~~~
  
#Follow 3 or 4 if problems occurred during code push from local to git(git push -u origin master)

**3.If User not added into local pc(Adding new users in local PC)**
  ~~~
  git config --global user.email "you@examole.com"
  git config --global user.name "Your name"
  git push -u origin master
  Then popup window will open, asking for git username and passwword
  ~~~

Check list of user if added duplicate and remove/replace

  ~~~
  git config --list
  git config --global --replace-all user.email "you@examole.co"
  git config --global --add user.email "you@examole.co"
  ~~~
  
  

**4.Remove/add user into computer for Windows**
~~~
Control panel > useraccount >credential >Generic credential
Next Remove the github key
and again add user into cmd 
~~~
  

########################
~~~
mkdir my_project (create folder)
cd my_project
touch .gitignore (create file)
git init
git add .
git commit -m "Initial commit"
git remote add origin youruser@yourserver.com:/path/to/my_project.git
git push origin master
~~~
##########################


**Url :localhost:8080 **
Input request
```json
{
"name": "username",
"email": "email"
}
```
   
