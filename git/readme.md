## Git Hidden Folder
```
For making these type of boxes, use triple starting and ending backsticks(`) present beside 1
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
git add . 
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

## Commits

## Branches

## Remotes

## Stashing

## Merging