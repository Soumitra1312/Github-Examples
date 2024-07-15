## Git Hidden Folder
```
For making these type of boxes, use triple starting and ending backsticks(`) which is present beside 1
```

```sh
Hidden folders are accessed using ls -la
```

There is a hidden folder called `.git` which tells you that our project is a git repo.

If we wanted to create a git repo in new project we' create the folder and then initialize that repo using `git init`

```
mkdir /workspaces/tmp/new-project
cd workspace/tmp/new-project
git init
touch readme.md
code Readme.md
git status
git add Readme.md 
# makes changes to readme.md
git commit -m "add readme file"
```

## Cloning

We can clone in three ways : HTTPS, SSH, Github CLI

Since we are using Github Codespaces we'll create a temporary directorey in our workspace

```sh
mkdir workspace/tmp
cd tmp
```

## HTTPS

```sh
git clone https://github.com/Soumitra1312/Github-Examples.git
cd Github-Examples
```
> You'll need to generate a Persoanl Access Token (PAT) for enhanced security while using Github locally.
> Personal Access Token can be used in place of passwords.
```sh
https://github.com/settings/token
```

### SSH
```ssh
git clone git@github.com:Soumitra1312/Github-Examples.git
cd Github-Examples
```

## Commits

When we want to commit code we can write git commit which will open up the commit edit message in the editor of choice.

```sh 
git commit
```

This line is used to set the default editor i.e Set the default editor.
``` 
git config --global core.editor emacs
```

Make a commit and commit message without opening an editor 

``` sh
git commit --m "add another exclamation mark"
```

## Branches

## Remotes

## Stashing

## Merging

## Add

When we want to stage changes that will be included in the commit, we can use the . to add all the possible files .

```
git add Readme.md
git add . 
```

## Reset

Reset allows you to move Staged changes to be unstaged.
This is useful when you want to revert all files not to be commited.

```
git add . 
git reset
```

> git reset will revert a git add . 

## Status

Git status will show you what files will or will not be commited.

```sh
git status
```

## Gitconfig file
The gitconfig file is what stores your global configurations for git such as email, name, editor and more.

Showing the contents of ```.gitconfig``` file 

```
git config --list 
```

When you first install git on a machine you are supposed to set up your name and email

```sh
git config --global user.name "John Doe"
git config --global user.email "johndoe@example.com"  
```

## Log
git log will show recent git commits to the git tree 

```sh
git log
```

## Push

When we want to push a repo to our remote origin

```
git push
```

## Delete
For deleting a folder
```sh
rm -rf foldername
```
For deleting a file
```sh
rm Readme.md
```
