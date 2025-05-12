# Git & GitHub Notes
# Basic Git Workflow (Pushing to GitHub)
-------------------------------------------------------------------------------------
1:-Initialize Git repo:
git init

2:-Add all files to staging:
git add .

3:-Commit changes:
git commit -am "commit message"

4:-Add remote origin:
git remote add origin [repository_url]

5:-Verify remote:
git remote -v

6:-Push to main branch:
git push origin main
----------------------------------------------------------------------------------------------------
# Cloning a Repository
git clone [repository_url]
----------------------------------------------------------------------------------------------------
# Creating New Project/Files

1:-Create folder:
mkdir folder_name

2:-Navigate into folder:
cd folder_name

3:-Create files:
touch filename.extension

4:-Check files:
ls

5:-Initialize Git:
git init

6:-Add changes:
git add .

7:-Commit:
git commit -m "message"

8:-Add remote:
git remote add origin [repository_url]

9:-Check branch:
git branch
(If master: git branch -M main to rename)

10:-Verify remote:
git remote -v

11:-Push:
git push origin main

12:-Check status:
git status
-----------------------------------------------------------------------------------------------
# Branching
1:-Check branches:
git branch

2:-Rename branch:
git branch -M new_name

3:-Create new branch:
git checkout -b branch_name

4:-Switch branches:
git checkout branch_name

5:-Delete branch:
git branch -d branch_name
(Must exit branch first)
--------------------------------------------------------------------------------------------
# Branch Workflow & Merging
* Work happens in separate branches (main vs feature branches)

* After completing work in feature branch:

* Create Pull Request on GitHub

* Compare changes (base: main ← compare: feature)

* Merge Pull Request

* Sync local repo after GitHub merge:

* git checkout main

* git pull origin main

# Optional cleanup:

* git branch -d feature (delete local branch)
---------------------------------------------------------------------------------------------
# Forking
Forking creates your personal copy of someone else's repo

Lets you make changes without affecting original project

Common workflow: Fork → Clone → Make changes → Push → Create PR to original repo