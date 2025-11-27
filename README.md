# GitHub
👉 "Hands-on Git &amp; GitHub practice repository covering essentials, advanced commands, workflows, and real DevOps use cases."

Setting Up Code Repository in GITHUB:
---------------------------------------
1. Goto www.github.com & Create an Account.
2. Create New Repository as "CentralGit"
3. Description : Centralized Repository
4. Choose Public.
5. Create Repository

Install & Configure Git:
------------------------
1. sudo su
2. yum update -y
3. yum install git -y
4. git --version
5. git config --global user.name "<region_specific_username>"
6. git config --global user.email "<your_email@example.com>"
7. git config --list

Workflow of Git:
------------------------

<img width="400" height="284" alt="image" src="https://github.com/user-attachments/assets/ea01b82f-47f3-40da-ac04-2ee8d36aa305" />


Git Lifecycle Explanation
-------------------------
1. Working Directory → (git add) → Staging Area 
2. Staging Area → (git commit) → Local Repository 
3. Local Repository → (git push) → Remote Repository (GitHub)

✅ 1. Basic Git Commands
------------------------
**Initialize a new Git repository**
* git init

**Clone a remote repository**
* git clone <repo-url>

**Check file changes in working directory**
* git status

**Add a specific file to staging area**
* git add <file>

**Add all files to staging area**
* git add .

**Commit staged changes with message**
* git commit -m "message"

**Push commits to remote repository**
* git push

**Push code to a specific branch**
* git push origin <branch>

**Pull latest changes from remote repository**
* git pull

**Download changes without merging**
* git fetch

**Show configured remote URLs**
* git remote -v

✅ 2. Branching Commands
------------------------
**List all branches**
* git branch

**Create a new branch**
* git branch <branch-name>

**List all local + remote branches**
* git branch -a

**Switch to another branch**
* git checkout <branch>

**Create and switch to a new branch**
* git checkout -b <branch>

**Modern switch command**
* git switch <branch>
* git switch -c <branch>

**Delete branch**
* git branch -d <branch>

**Force delete branch**
* git branch -D <branch>

✅ 3. Merge & Rebase
--------------------
**Merge another branch into current branch**
* git merge <branch>

**Rebase current branch on another branch**
* git rebase <branch>

**Continue rebase after fixing conflicts**
* git rebase --continue

**Abort rebase**
* git rebase --abort

✅ 4. Log & History
-------------------
**Show full commit history**
* git log

**Show one-line history**
* git log --oneline

**Visual graph of branches**
* git log --graph

**Show commit with decorations (branch names, tags)**
* git log --decorate

**Show what changed in a specific commit**
* git show

✅ 5. Stash Commands
--------------------
**Save work without committing.**
* Save working changes
* git stash

**Save with message**
* git stash save "message"

**List all stash entries**
* git stash list

**Apply stash but keep it**
* git stash apply

**Apply stash and remove it**
* git stash pop

**Delete a specific stash**
* git stash drop

**Clear all stashes**
* git stash clear

✅ 6. Undo Changes
------------------
**Restore file from latest commit**
* git restore <file>

**Unstage a file**
* git restore --staged <file>

**Reset commits (soft: keep changes staged)**
* git reset --soft HEAD~

**Reset commits (mixed: keep working changes)**
* git reset --mixed HEAD~

**Reset commits (hard: delete all changes)**
* git reset --hard HEAD~

**Undo a commit with a new commit**
* git revert <commit-id>

**Remove untracked files**
* git clean -f

**Remove untracked files + folders**
* git clean -fd

✅ 7. Remote Commands
---------------------
**Add a remote repo**
* git remote add origin <url>

**Remove remote**
* git remote remove origin

**Rename remote**
* git remote rename origin neworigin

✅ 8. Tagging Commands
----------------------
**List all tags**
* git tag

**Create a tag**
* git tag <tag-name>

**Create an annotated tag**
* git tag -a <tag-name> -m "message"

**Push a single tag**
* git push origin <tag-name>

**Push all tags**
* git push origin --tags

**Delete tag**
* git tag -d <tag-name>

✅ 9. Diff (Compare Changes)
----------------------------
**Show unstaged changes**
* git diff

**Show staged changes**
* git diff --staged

**Compare two branches**
* git diff <branch1> <branch2>

**Compare two commits**
* git diff <commit1> <commit2>

✅ 10. Cherry-Pick
------------------
**Copy a commit from another branch**
* git cherry-pick <commit-id>

**Continue cherry-pick after fixing conflicts**
* git cherry-pick --continue

**Abort cherry-pick**
* git cherry-pick --abort

✅ 11. Git Configuration
------------------------
**Set username**
* git config --global user.name "<name>"

**Set email**
* git config --global user.email "<email>"

**Show all config**
* git config --list


