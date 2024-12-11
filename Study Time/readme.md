## git hidden folder
ls -la
there is a hidden folder called .git which tells you that your project is a git repo.

if you what to create a git repo in a new project we  create a folder  and then initialize that repo using git init.

```
mkdir/ workspaces/tmp/new-project
cd workspaces/tmp/new-project
git init
touch Readme.md
code Readme.md
git status
git add .
git status

git reset

git add Readme.md

# make changes to Readme.md

git commit -m "add Readme file"

```


## cloning

we can clone 3 ways :HTTPS, SSH, GITHUB CLI
Since we are using github codespaces, will create a temporery direcrry in our worke space

```sh
mkdir /workspace/tmp
cd/ workspace/ tmp
```

ls - la :- for getting all the hidden files
### HTTPS
```sh
git clone https://github.com/AmalVinob/Github-LearningENV.git

cd/ Github-LearningENV 
``` 

>one way of doing commit is to get access token (personel access token) from the settings and 
>you will use PAT as password when login



### ssh

## commit

when we want to commit code we write git commit which will open
up the commit edit message in the editor of choice
```sh
git commit
```

set the global editor
```
$ git config --global core.editor emacs
```
Make a commit and commit wiht message without opening editor


```sh
git commit -m "hellow world added"
```

## Branchs



## Remotes

## Stashing

## Merging

## Add
when you want to stage changes that will be included in commit,
we can use . to add all the  possible files.

```
git add Readme.md
git add .

```

## Reset

reset allow you to move staged changes to be unstaged.
This is usefull when you dont want all files to be not commited

```
git add .
git reset
```
Revert add changes

## git ststus

git status shows you what files will or willnot commited

```
git status
```

## git config file
git config file is  what stores your global configurations  for git such as email, name, editor and more.

```
git config --list
```
show the conted of the .gitconfig file

When you first install Git on your machine you are suppose to set up your name and email

```sh
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
```


## push

When we want to push a repo to our remote orgin 

```sh
git push
```