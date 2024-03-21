+++
title = 'Git Commands'
date = 2024-03-21T02:30:01-04:00
draft = false
+++

I often find myself forgetting the basic commands for Git. I know it's dumb but it's just easy to keep all of them in one place for reference. 

Also, for anyone new to Git - these are all the commands you need to get started. 


```bash
git init # command to convert any folder to a git repo. It creates a .git folder inside and then git tracks the changes made in it.

git add <filename> # used to put the changes into staging area.

git add . # add all files in the repo

git status # check the state of branches and repo

git diff # check the difference between last commit and unstaged changes

git commit -m "message" # all files that were added using git add are committed

git checkout -b <branchname> # create a new branch to make changes to it.

git checkout <branchname> # go to the branchname

git merge # merges changes into the current branch

git remote add origin <url> # add github remote repo to the folder

git remote remove origin # remove remote repo connection from the local

git push -u origin main # -u saves the setting. git push pushes to main

```

> One challenge that I faced was that my email could've been exposed but GitHub has a setting that needs to be unchecked for that. Instead, I changed my email according to what GitHub suggested.

```bash
git config --global user.name # tells what is the user name that will show in GitHub
git config --global user.name "KP" # Sets the username to KP in GitHub
git config --global user.email # tells what is the user name that will show in GitHub
git config --global user.email "abc@gmail.com" # sets the email to abc@gmail.com in GitHub
```

```bash
git pull origin main # to get changes from remote to local main

git push # send the changes to remote repo from local main

git push origin new # pushing changes in "new" branch to remote (GitHub)
```

```bash
git reset --soft HEAD~1 #removes a commit and takes the changes done in the commit back to staging
```

> GitIgnore Related Stuff:
> Create a file called ".gitignore"
> Add "folder/" - Add folder and its content to gitignore file

```bash
git rm --cached -r .venv # remove .venv folder from git tracking

```

```bash
# List all tracked files
git ls-files

# List all tracked files in the current directory
git ls-files .

# List all tracked files in the current directory and all subdirectories
git ls-files -r

# List all tracked files that have been changed since the last commit
git ls-files --modified

# List all tracked files that have been added since the last commit
git ls-files --other

# List all tracked files that have been deleted since the last commit
git ls-files --deleted
```

