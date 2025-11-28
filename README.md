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
```
Initialize a new Git repository
* git init
```

```
Clone a remote repository**
* git clone <repo-url>
```

```
Check file changes in working directory**
* git status
```

```
Add a specific file to staging area**
* git add <file>
```

```
Add all files to staging area**
* git add .
```

```
Commit staged changes with message**
* git commit -m "message"
```

```
Push commits to remote repository**
* git push
```

```
Push code to a specific branch**
* git push origin <branch>
```


```
Pull latest changes from remote repository**
* git pull
```


```
Download changes without merging**
* git fetch
```

```
Show configured remote URLs**
* git remote -v
```

✅ 2. Branching Commands
------------------------
```
List all branches**
* git branch
```

```
Create a new branch**
* git branch <branch-name>
```

```
List all local + remote branches**
* git branch -a
```

```
Switch to another branch**
* git checkout <branch>
```

```
Create and switch to a new branch**
* git checkout -b <branch>
```

```
Modern switch command**
* git switch <branch>
* git switch -c <branch>
```

```
Delete branch**
* git branch -d <branch>
```

```
Force delete branch**
* git branch -D <branch>
```

✅ 3. Merge & Rebase
--------------------
```
Merge another branch into current branch**
* git merge <branch>
```

```
Rebase current branch on another branch**
* git rebase <branch>
```

```
Continue rebase after fixing conflicts**
* git rebase --continue
```

```
Abort rebase**
* git rebase --abort
```

✅ 4. Log & History
-------------------
```
Show full commit history**
* git log
```

```
Show one-line history**
* git log --oneline
```

```
Visual graph of branches**
* git log --graph
```

```
Show commit with decorations (branch names, tags)**
* git log --decorate
```

```
Show what changed in a specific commit**
* git show
```

✅ 5. Stash Commands
--------------------
```
Save work without committing.**
* Save working changes
* git stash
```

```
Save with message**
* git stash save "message"
```

```
List all stash entries**
* git stash list
```

```
Apply stash but keep it**
* git stash apply
```

```
Apply stash and remove it**
* git stash pop
```

```
Delete a specific stash**
* git stash drop
```

```
Clear all stashes**
* git stash clear
```

✅ 6. Undo Changes
------------------
```
Restore file from latest commit**
* git restore <file>
```

```
Unstage a file**
* git restore --staged <file>
```

```
Reset commits (soft: keep changes staged)**
* git reset --soft HEAD~
```

```
Reset commits (mixed: keep working changes)**
* git reset --mixed HEAD~
```

```
Reset commits (hard: delete all changes)**
* git reset --hard HEAD~
```

```
Undo a commit with a new commit**
* git revert <commit-id>
```

```
Remove untracked files**
* git clean -f
```

```
Remove untracked files + folders**
* git clean -fd
```

✅ 7. Remote Commands
---------------------
```
Add a remote repo**
* git remote add origin <url>
```

```
Remove remote**
* git remote remove origin
```

```
Rename remote**
* git remote rename origin neworigin
```

✅ 8. Tagging Commands
----------------------
```
List all tags**
* git tag
```

```
Create a tag**
* git tag <tag-name>
```

```
Create an annotated tag**
* git tag -a <tag-name> -m "message"
```

```
Push a single tag**
* git push origin <tag-name>
```

```
Push all tags**
* git push origin --tags
```

```
Delete tag**
* git tag -d <tag-name>
```

✅ 9. Diff (Compare Changes)
----------------------------
```
Show unstaged changes**
* git diff
```

```
Show staged changes**
* git diff --staged
```

```
Compare two branches**
* git diff <branch1> <branch2>
```

```
Compare two commits**
* git diff <commit1> <commit2>
```

✅ 10. Cherry-Pick
------------------
```
Copy a commit from another branch**
* git cherry-pick <commit-id>
```

```
Continue cherry-pick after fixing conflicts**
* git cherry-pick --continue
```

```
Abort cherry-pick**
* git cherry-pick --abort
```

✅ 11. Git Configuration
------------------------
```
Set username**
* git config --global user.name "<name>"
```

```
Set email**
* git config --global user.email "<email>"
```

```
Show all config**
* git config --list
```

**Git ignore**
--------------
```
.gitignore tells Git which files to ignore.
It stops unwanted files from being added or committed.
```

**Steps :**
-----------
1. Create a file " .gitignore "
2. give the pattern of filenames you dont want to commit 
3. Add and commit .gitignore file 
4. Create some files with extensions you dont want to commit 
5. Run git add . command to confirm if git ignore works or not.

```
Ex:
		1. nano .gitignore 
			<inside .gitignore file put the filenames pattern to ignore those files>
			*.class
			*.bin 
			*.txt
			*.tests

		2. Save the file and commit this file

		3. git add .gitignore

		4. git commit -m "ignore file added"

		5. create some class files, bin files and some text files and try to add them. (touch file{1,2,3}.{class,bin,txt,tests,java,py} this command will create 5 class,bin,txt,tests,java,py files

		6. add all these files at once and check the working of gitignore 
			$git add .

		7. Check status 
			$git status

		8. You should see only java and py files are staged and they only will
			be eligible for commit.
```


Git Branching Strategy:
---------------------------
Branching is required when you want to work on a new feature or task or want to keep a backup without disturbing production code.
 
```
To see list of available branches:
git branch
```

```
To create a new branch :
git branch <branch name>
```

```
To switch branch 
git checkout <branchname_you_want_to_goto>
```

* Create some new files and check the status and files in both branches
* To commit the changes to particular branch, 
* Be in that branch and commit.
* When not committed, the files will be floating in 
* The entire workspace and will be visible to all
* Other branches in your local repo.

**How is branch created?**
* The new branch is always created from the current branch you are working in.
* When you do git branch, the same working copy of current branch is copied to new branch and now onwards whatever you do in this new branch will be personal to this branch.
* The new branch will contain all the previous work and your new work. 
* NEW BRANCH = PARENT_BRANCH_COPY + NEW_WORK 

**Git MERGE :**
---------------
1. when we are done finishing our work on any new feature, we need to merge to master or production branch.
2. To merge any branch to any other branch :
	- be in the recieving branch 
	- run the command :
```
git merge <source_branch_name>
```
3. Verify the merge
```
git log
``` 
4. Push to central repo
```
git push origin master
``` 
6. This will merge your new branch with current branch (can be master or any other branch)

**Git Conflict**
----------------
When same file having different content in different branches, if you do merge, then conflict occurs.

In this case you need to resolve the conflict and add and commit again.

Remember : conflict occurs during "merging" process.
				when we do git merge or git pull, conflict occurs.

**How to resolve git conflict?**
-------------------------------
1. Check which file has a merge conflict
```
git status 
```
2. Open the file 
	- Decide what content to keep 
	- Remove other content which is not required
3.  Add and Commit 
				
