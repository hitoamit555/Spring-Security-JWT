# Spring-Security-JWT
SpringBoot Security with JWT

**End point Url :# localhost:8080/login**
~~~
Username: username
Password: password
~~~
#Output
~~~
Done (Controller Output)
~~~

#Input json request(TODO:)
```json
{
"name": "username",
"email": "email"
}
```

**Git Commands and step to create new repo first time**

**1. Goto git browser and create repo with same name as local created. And copy url of you Repo and follow cmd below.**

**2. Goto local PC and follow below cmd**
  ~~~ 
  cd my_project
  git init
  git add .
  git commit -m "Initial commit"
  git remote add origin youruser@yourserver.com:/path/to/my_project.git
  git push -u origin master(Before push anything,always do pull first:git pull origin master)
  ~~~
  
***Follow 3 or 4 if problems occurred during code push from local to git(During: git push -u origin master)***

**3.If User not added into local pc(Adding new users in local PC)**
  ~~~
  git config --global user.email "you@examole.com"
  git config --global user.name "Your name"
  git push -u origin master
  Then popup window will open, asking for git username and password
  ~~~

Check listof users if added duplicate and remove/replace

  ~~~
  git config --list
  git config --global --replace-all user.email "you@examole.co"
  git config --global --add user.email "you@examole.co"
  
  git remote -v(check remote url set or not if not below)
  git remote set-url origin git@github.com:USERNAME/REPOSITORY.git
  ~~~
  
  

**4.Remove user from computer as below and try #3 again**
~~~
Control panel > useraccount >credential >Generic credential
Next Remove the github key
and again add user into cmd 
~~~
  

########################
~~~
mkdir my_project (create folder)
cd my_project
touch .gitignore (create file and add entry those file don't want to track/commit into git)
git init
git add .
git commit -m "Initial commit"
git remote add origin youruser@yourserver.com:/path/to/my_project.git
git push origin master
~~~
##########################

**Git command if don't want to genrate new commit id(Amend into same PR)**
~~~
git add -u
git commit --amend
esc + : + wq  (save file as prev comments) /(Don't save: esc + : + q)
git push -f origin yourBranch (-f :fource push need)
~~~

**Git resolve conflict #1 and #2 scenario**

~~~
Conflict: Occures When,In the same file,same time ,same code block changed by multiple users

#1 (Conflict while take update)
git pull origin master (always do after commit you local changes )
Identify how many files have conflict(Red one) -Resolve the conflicts/Do the local changes/Keep either one changes
#Best Way, copy entaire file change from Master branch of git UI/Console past into conflict file 
and Add your changes on top of that.Do for All file one by one
git add -u
git commit -a(git commit -m "your's comments")
git push origin mybranch(git push -f origin mybranch) 

#2(Conflict while merging)
git reset --hard origin/myBranch
git pull origin master
#Best Way follow from above
git add -u
git commit -a
git push origin mybranch

~~~


**First time working on Any New Changes /Daily update to avoid conflict**
~~~
git clone url(Url can copy from git repo )

It can clone by 2 ways.
1.SSH key Ways:Genrate sshkey locally and add into git console in key and add into .profile(In MAC)
2.Add user into local PC (Follow #3 or #4 as above.In Windows)

git checkout master/myBranch
git reset --hard origin/master
git pull origin master
git checkout -b myNewbranch
git add -u
git commit -m "my comments"
git pull origin master(Always do before push into repo,after local commit)
git push origin myNewbranch
Note:(Before push anything after commit,always do pull first and then push:git pull origin master)
~~~

**All useful cmd**
~~~
git branch -D myBranch
git stash .
git stash apply
git status
git diff 
git chckout fileWithProjectPath(remove file from stage/commit)
git add -u(Add only tracked file into stage/commit)
git add .(all tracked and untracked)
git add fileWithProjectpath
git log -4
git charry-pick commitID(To get changes into you branch by commitId)
git rebase origin/master

If you wish to set tracking information for this branch you can do so with:
git branch --set-upstream new origin/<branch>
~~~

   
