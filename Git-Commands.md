# Git \& GitHub Commands Cheat Sheet (QA Engineer)





###### 1\. Git Installation

* git --version → Check the installed Git version.



###### 2\. Git Configuration

* git config --global user.name "Your Name" → Set Git username.
* git config --global user.email "your@email.com" → Set Git email.
* git config --list → View all Git configuration settings.



###### 3\. Repository

* git init → Create a new local Git repository.
* git clone <repository-url> → Copy an existing repository from GitHub.



###### 4\. Check Status

* git status → View modified, staged, and untracked files.



###### 5\. Stage Changes

* git add filename → Stage a specific file.
* git add . → Stage all changed files.



###### 6\. Commit Changes

* git commit -m "message" → Commit staged changes.
* git commit -am "message" → Stage and commit tracked files in one step.



###### 7\. View History

* git log → Show detailed commit history.
* git log --oneline → Show short commit history.
* git log --graph --oneline --all → Show commit history with branch graph.



###### 8\. Compare Changes

* git diff → View unstaged changes.
* git diff --staged → View staged changes.



###### 9\. Branch Management

git branch → List local branches.

git branch branch-name → Create a new branch.

git switch branch-name → Switch to another branch.

git switch -c branch-name → Create and switch to a new branch.

git branch -d branch-name → Delete a merged branch.

git branch -D branch-name → Force delete a branch.

git branch -m new-name → Rename the current branch.



###### 10\. Merge

* git merge branch-name → Merge the specified branch into the current branch.



###### 11\. Remote Repository

* git remote -v → View remote repositories.
* git remote add origin <repository-url> → Add a remote repository.
* git remote remove origin → Remove a remote repository.
* git remote set-url origin <repository-url> → Change the remote URL.



###### 12\. Push

* git push → Push commits to the remote repository.
* git push -u origin main → First push and set upstream branch.
* git push origin branch-name → Push a specific branch.
* git push --force → Force push (use with caution).



###### 13\. Pull

* git pull → Download and merge remote changes.
* git pull origin main → Pull changes from a specific branch.



###### 14\. Fetch

* git fetch → Download remote changes without merging.
* git fetch --all → Fetch all remote branches.



###### 15\. Stash

* git stash → Temporarily save uncommitted changes.
* git stash list → View saved stashes.
* git stash apply → Apply the latest stash.
* git stash pop → Apply and remove the latest stash.
* git stash drop → Delete a stash.
* git stash clear → Delete all stashes.



###### 16\. Undo Changes

* git restore filename → Discard changes in a file.
* git restore --staged filename → Unstage a file.
* git reset --soft HEAD\~1 → Undo the last commit and keep changes staged.
* git reset --mixed HEAD\~1 → Undo the last commit and unstage changes.
* git reset --hard HEAD\~1 → Delete the last commit and all changes.



###### 17\. Revert

* git revert <commit-id>` → Safely undo a commit by creating a new commit.



###### 18\. Remove Files

* git rm filename → Delete a tracked file.
* git rm --cached filename → Stop tracking a file but keep it locally.



###### 19\. Tags

* git tag → List all tags.
* git tag v1.0 → Create a new tag.
* git push origin --tags → Push all tags.



###### 20\. Clean Repository

* git clean -n → Preview files that will be removed.
* git clean -f → Delete untracked files.
* git clean -fd → Delete untracked files and folders.



###### 21\. Useful Commands

* git branch --show-current → Show the current branch.
* git rev-parse HEAD → Show the current commit ID.
* git rev-parse --show-toplevel → Show the repository root directory.
* git ls-files → List all tracked files.



###### 22\. Daily Workflow



1\. git status → Check current changes.

2\. git pull → Get the latest code.

3\. Make your changes.

4\. git add . → Stage changes.

5\. git commit -m "message" → Commit changes.

6\. git push → Upload changes to GitHub.



###### 23\. QA Automation Workflow

1\. git clone <repository-url> → Clone the project.

2\. git switch develop → Switch to the develop branch.

3\. git pull origin develop → Get the latest code.

4\. git switch -c feature/login-test → Create a feature branch.

5\. Write or update test scripts.

6\. git add .

7\. git commit -m "Added login automation tests"

8\. git push -u origin feature/login-test

9\. Create a Pull Request (PR).

10\. After merge, delete the feature branch.



