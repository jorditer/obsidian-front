## Commiting

`git commit -am "<msg>"` adds and commits at the same time. `-a = --all` (stage all, except new untracked files). You can create an alias to work faster `git config --global alias.<aliasname> "commit -am` Now when you run `<aliasname>` it will do all the work

`git commit --amend -m "newmessage"` Replaces message of last commit

## Add files to last commit
```zsh
git add .
git commit --amend --no-edit
```

```js
git init //Initializes project
git init -b <branchname> //Initializes project and names the inital branch
git status // Status of changes
git add filename // Stages filename. git add . // All txt files git add *.txt
git commit -m message // Commits staged files into the repository
git log // Shows commits chronologically git log --oneline // Shows logs in oneline
git checkout HEAD filename // Restores last filename commit
git mv <name> <rename>
git rm <name>
git branch // Shows all branches
git branch <newBranch> // creates <newBranch>
git checkout <branchname> // switches to branchname
git checkout -b <branchname> // creates and switches to branchname
git merge <branchname> // Merges current branch with main
git branch -d <branchname> // Delete branch. Must be used once the branch is merged
git branch -D <branchname> // Delete branch that WAS NOT merged into main
git clone <location> <clonename> //clonename=name of the directory in which to clone
git fetch // clones changes in a branch
git merge origin/master
git push origin <branchname> // Shares your work to the remote origin
git remote -v // Shows location of
git rebase main // Reapplies commits on top of another base branch DONT USE IN MAIN
git log --graph --decorate --oneline --all
git pull //updates from remote rep, convination off git fetch and git merge
git diff // Shows difference between working and staging
git diff --staged
git diff 0x37233 0x38942 // diff between 2 commits
git diff branchOne branchTwo
git checkout <commit-hash> // Go back to a previous hash, use git checkout <branch-name> to restore, or git reflog
git stash
git stash pop // bring back changes
git stash apply // apply changes



##Pull requests
Follow a Pull Request Structure – What, Why, and How?

## push
git remote add origin https://github.com/jorditer/remove-duplicates.git
git remote -v // Shows fetch and push links
git push -u origin main   // -u sets upstream so that you can now use just git push and it will automatically push form main to origin
git push <remote> <branch>

## fetch
git pull // Gets info into your work area 
git fetch // Like git pull but it doesn't add the info into your work area git pull = git fetch + git merge
git pull origin main

##.git ignore
src/main.js // relative paths
*.html      // ignores all .html files, regex
example*    // ignores all files that startwith example
!example.css// except example.css, doesn't work for files inside a negated directory
src/v[1-3]/**/*.log // ignores all .log files inside the v1, v2, v3 folders


```