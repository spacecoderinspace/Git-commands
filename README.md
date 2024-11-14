# Git-

1. Basic Git Workflow Commands  
   • `git clone <repository-url>`: Clones a remote repository to your local machine, often used at the start of a project.  
   • `git status`: Shows the status of your working directory and staging area, displaying changes to be committed or files not yet staged.  
   • `git add <file>` / `git add .`: Stages changes for the next commit. `git add .` stages all modified files.  
   • `git commit -m "commit message"`: Commits staged changes to the local repository. Good commit messages are critical, especially in collaborative projects.  
   • `git push`: Pushes committed changes from your local repository to the remote repository (e.g., GitHub, Azure Repos).  
   • `git pull`: Fetches changes from the remote repository and merges them with your local branch, keeping your code up to date with others' work.  

2. Branching and Merging  
   • `git branch <branch-name>`: Creates a new branch. Branches are essential in data engineering to work on features, bug fixes, or experimental changes without affecting the main codebase.  
   • `git checkout <branch-name>`: Switches to the specified branch. It’s common to have different branches for development, staging, and production.  
   • `git merge <branch-name>`: Merges the specified branch into your current branch. Used to combine changes from different branches, especially for feature branches into a main or dev branch.  
   • `git rebase <branch-name>`: Re-applies commits from one branch onto another. Rebasing can be useful for maintaining a cleaner commit history but requires careful usage to avoid conflicts.  

3. Collaboration and Conflict Resolution  
   • `git fetch`: Retrieves updates from the remote repository without merging them, allowing you to see if your branch is behind before deciding to pull.  
   • `git diff`: Shows the differences between your working directory and the latest commit or between branches. This is useful for reviewing changes before committing.  
   • `git stash`: Temporarily stores your local changes, which can be helpful if you need to switch branches without committing incomplete work.  
   • `git stash apply`: Reapplies stashed changes after switching branches.  
   • `git log`: Shows the commit history, which is helpful for tracking changes, especially in collaborative environments.  
   • `git reset`: Used to undo changes, with variations like `--soft`, `--mixed`, or `--hard` to control whether changes are unstaged or deleted entirely.  

4. Working with Remote Repositories  
   • `git remote add <name> <url>`: Adds a remote repository, allowing you to link your local repository with an online platform like GitHub or Azure Repos.  
   • `git pull origin <branch>`: A combination of fetch and merge, it pulls updates from a specific branch on the remote.  
   • `git push origin <branch>`: Pushes a local branch to the remote repository. In many workflows, pushing to branches and creating pull requests (PRs) for review is a common practice.  

5. Reviewing and Reverting Changes  
   • `git checkout <file>`: Reverts a specific file to the last committed state, discarding local changes.  
   • `git revert <commit-id>`: Creates a new commit that undoes a specific commit without rewriting commit history, useful for safely reversing changes.  
   • `git cherry-pick <commit-id>`: Applies changes from a specific commit to your current branch, often used to apply hotfixes.  

6. Tagging and Releases  
   • `git tag <tag-name>`: Creates a tag for a specific commit, often used for marking release versions.  
   • `git push origin <tag-name>`: Pushes tags to the remote repository, allowing you to publish tagged versions, which is helpful for version control and CI/CD deployments.  
