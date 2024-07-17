## README: Git Workflow Steps

This document outlines a basic Git workflow for managing branches and pushing changes to a remote repository.

### Step-by-Step Git Workflow

#### 1. Create a New Branch

Create and switch to a new branch `feature-branch`:

```bash
git branch feature-branch       # Create a new branch
git checkout feature-branch     # Switch to the new branch
```
Alternatively, you can combine the above two commands into one:

```bash
git checkout -b feature-branch
```

#### 2. Stage and Commit Changes
Add all changes in the current directory to the staging area and commit them with a descriptive message:

```bash
git add .                       # Stage all changes
git commit -m "comments"        # Commit changes with a meaningful message
```
#### 3. Fetch and Rebase
Fetch the latest changes from the remote repository (origin) and rebase your local branch (feature-branch) on top of origin/main:

```bash
git fetch origin                # Fetch latest changes from origin
git rebase origin/main          # Rebase feature-branch on origin/main
```
#### 4. Push Changes to Remote
Push your local feature-branch to the remote repository (origin). Use --force-with-lease to safely force-push if needed:

```bash
git push origin feature-branch --force-with-lease   # Push changes to remote feature-branch
```

#### 5. Merge Changes to main
Switch back to the main branch and merge feature-branch into main:

```bash
git checkout main               # Switch to main branch
git merge feature-branch        # Merge feature-branch into main

```

#### 6. Push Changes to main Branch
Finally, push the merged changes in main to the remote repository:

```bash
git push origin main            # Push changes to remote main branch

```

### Summary

This Git workflow guides you through creating a new branch, making and committing changes, syncing with the remote repository, and merging those changes back into the main branch. Always ensure to fetch and rebase before pushing to keep your branch up-to-date with the remote changes.
