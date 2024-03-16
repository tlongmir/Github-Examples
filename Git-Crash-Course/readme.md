## Commits
> You'll need to generate a personal access token (PAT)
https://github.com/settings/token

You will use PAT as your password when you login
- Give it access to contents for commits
- SSH 
mkdir /workspaces/tmp/new-project
cd /workspaces/tmp/new-project
git init
touch Readme.md
nano or vim Readme.md
git status
git add Readme.md

When we want to commit code we can write git commit which will open up the commit edit message in the editor of choice.

```sh
git commit

```
Set the global editor
```
git config --global core.editor nano
```
Make a commit and commit without editor
```sh
git commit -m "add another exclamation"
```
## SSH
git clone @github.com:tlongmir/Github-Examples.git
cd Github-Examples

ssh-keygen -t rsa
github-alt_id_rsa


# Make changes
git commit -a -m "Add readme file"

## Cloning
Since we are using GitHub codespaces we'll create a temporary directory in our work

```sh
mkdir /workspace/tmp
cd /workspace/tmp
```

## HTTPS
```sh
git clone https://github.com/tlongmir/Github-Examples.git
```
## Branches

List of Branches

```
git branch
```

Create a new branch
```
git branch branch-name
```

Checkout the branch

```
git checkout dev
```

## Remotes

## Stashing

## Merging

## Add
stage changes
```
git add Readme.md
git add .
```
## status
shows you what files will or will not be staged

## Gitconfig file
The gitconfig file is what stores your global configurations for git such as email, name, editor and more.

Showing the contents of our .gitconfig file
```
git config --list --show-origin
```
```sh
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
```
## Log
git log will show recent git commits to the git tree

## Push
push a repo to remote origin
```
git push 
```

## Reset
Reset allows you to move staged changes to be unstaged. 
This is useful when want to revert all files not to be commited

```
git add .
git reset
```

> git reset will rever a git add .