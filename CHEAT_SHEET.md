# Git & GitHub Cheat Sheet (one page)

## The core loop
`edit files` => `git add` => `git commit` => `git push`

## Setup (once)
 Command => What it does 

 `git config --global user.name "Your Name"` => Set your name 
 `git config --global user.email "you@example.com"` => Set your email 

## Everyday commands
 Command => What it does 

 `git clone <url>` => Download a repo to your computer 
 `git status` => See what has changed 
 `git add <file>` / `git add .` => Stage a file / everything 
 `git commit -m "message"` => Save a snapshot with a message 
 `git push` => Send your commits to GitHub 
 `git pull` => Get the latest changes from GitHub 
 `git log --oneline` => See commit history 
 `git diff` => See what you changed 

## Branches
 Command => What it does 

 `git branch` => List branches 
 `git switch -c <name>` => Create and move to a new branch
 `git switch <name>` => Move to an existing branch 
 `git merge <name>` => Merge a branch into the current one 

## Pull request flow
1. Fork the repo
2. Clone your fork
3. Create a branch
4. Commit and push
5. Click **Compare & pull request** on GitHub

## Undo (use carefully)
 Command => What it does 

 `git restore <file>` => Throw away changes in a file 
 `git restore --staged <file>` => Unstage a file 
 `git commit --amend` => Edit your last commit message

## Merge conflicts
Git marks conflicts like this:
```
<<<<<<< HEAD
your version
=======
their version
>>>>>>> branch-name
```
Keep what you want, delete the markers, then `git add` and `git commit`.

## Git vs GitHub
**Git** is the tool on your computer that tracks changes. **GitHub** is the website that stores your repos online and lets people collaborate.