Repository for the testing / practicing w/ the GitHub Foundations course.

## Git Hidden Folder

There is a hidden folder called '.git' that tells you that the project is a Git Repo. If we wanted to create a git repository in a new project, we'd create the required folder(s) and then initialize the repository via `git init`.

```sh
mkdir /workspace/tmp/new-project
cd /workspace/tmp/new-project
git init
touch ReadMe.md
open ReadMe.md # Add relevant changes to readme.md
git status # This shows tracked / untracked files.
git add ReadMe.md # This adds "ReadMe.md" as a tracked file
git commit -a -m "add readme.md file"
```

## Cloning

- We can clone 3 ways.
-- HTTPS
-- SSH
-- GitHub CLI

Since we're using GitHub Codespaces, we'll create a temporary directory in our workspace.

```sh
mkdir /workspace/tmp
cd /workspace/tmp
```

### HTTPS

```md
- git clone https://github.com/JamesStrachanTyler/github-foundations.git
- cd github-foundations
- ls -la
```

### SSH

```md
- I'd generate a PAT (Personal Access Token) and apply to my local IDE. I can then clone a git repo using: `git@github.com:JamesStrachanTyler/github-foundations.git`
```

## Commits

When we want to commit code, we can write `git commit` which will open up the commit edit message in the code editor.

```sh
git commit
```

We can add a commit message using the command line via the following command, rather than having to open up the commit page and adding the message there.

```sh
git commit -m "Commit message"
```

## Branches

## Remotes

## Stashing

## Merging

## Add
When we want to add 

## Status
Git status shows what files will be / will not be committed.
```
git status
```

## Log
We can show recent git commits to the git tree via the following command:
```sh
git log
```

## Reset

Reset allows you to move staged changes back to unstaged. Useful when you only want to commit specific files and revert accidental stages.

```sh
git add .
git reset
```
> Git reset would revert the add all.

## Push
When we want to push our local repository to our remote origin (VCS), we can push 