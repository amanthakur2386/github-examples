# git hidden folder
There is a hidden folder called `.git` which tells you that our project is a git repo.

If we wanted to create a git repo in a new project we will create the folder and the initialise that repo using `git init`

```
mkdir /workspaces/tmp/new-project
cd /workspaces/tmp/new-project
git init
touch README.md
code README.md
git status
git add readme.md
# makes changes to README.md
git commit -a -m "addreadme file"
```

## cloning
we can clone in 3 ways: HTTPS, SSH, GITHUB CLI
Since we are using github codespace , we will create a temporary directory in our workspace
```sh
mkdir /workspaces/tmp
cd /workspaces/temp
```

## HTTPS

```md
git clone https://github.com/amanthakur2386/github-examples.git
cd github-examples
```

## commits

when we want to commit coe we can write git commit which will open up the commit edit message in the editor of choice.

```sh
git commit
```

Make a commit and commit message without opening an editor
```sh
git commit -m "add another exclamation"
```

## Add
When we want to stage changes that will be included in commit we can use the . to add all possible files
```
git add .
git reset
```

## reset
Reset allows you to move staged changes to be unstaged. Thsi is useful when you want to revert all files not to be commited.
```
git add .
git reset
```
> git reset will revert a git add .
## status
git status shows you what files will or will not be commited
```sh
git status
```
## log
Git log will show recent git commits to the git tree
```sh
git log
```
