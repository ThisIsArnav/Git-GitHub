# Git and GitHub

To link ur project to git and link it to github:
1) Run ``git init`` command in the project directory
2) Run ``git remote add origin`` + your ``https`` Example: ``git remote add origin https://github.com/ThisIsArnav/abcd.git``
  
  NOTE: You can get ur ``https`` like this: ``ur github repository url`` + ``.git`` at the end
  
 3) Run ``git add . && git commit -m Updated && git push``
 
# In case of error's while pushing the Git push:

try: ``git push -u origin master``


try: ``git push -f origin master`` this forcely pushes commits

# Git lfs

1) Track all the files using git lfs using this command:
``git lfs track``

2) Add files to the repo:
``git add .``

3) Commit the file and push it to GitHub:

```
$ git commit -m Updated
$ git push
```

4) Push to another with in git

Use fetch command in the local repo
```
$ git fetch
```
check that your branch has come to your local using

```
$ git branch
```
now change your branch using checkout

```
$ git checkout -b branch_name
```
do some changes then

```
$ git add .
$ git commit -m "message"
$ git push origin remote_branch_name
```
# Handling branches
**Commiting to a different branch of same repo**

Step-01: create and switch to the new branch B
```console
git checkout -b B
```

Step-02: Add changes in the new local branch

```console
git add . //or specific file(s)
```

Step-03: Commit the changes

```console
git commit -m "commit_message"
```

Step-04: Push changes to the new branch B. The below command will create a new branch B as well remotely

```console
git push origin B
```
