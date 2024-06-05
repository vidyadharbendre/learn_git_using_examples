# Additional Git Commands

This guide provides a list of additional Git commands for managing branches, viewing commit history, and merging changes.

## Step-by-Step Guide

### 1. View Commit History
- To see the commit history:
```bash
    git log
```
- To see a bried summary of the commit history:
```bash
    git log --oneline
```
- To view changes introduced by each commit:
```bash
    git log -p
```

### 2. Create and Switch to a New Branch
- To switch to an existing branch:
```bash
    git checkout <branch-name>
```

### 3. List All Branches
- To list all branches in your repository:
```bash
    git branch
```
- To list all branches, including remote branches:
```bash
    git branch -a
```
### 4. Merge a Branch into the Current Branch
- To merge changes from another branch into your current branch:

```bash
    git merge <branch-name>
```
- Resolve any conflicts that arise, then:
```bash
git add <file-name>
git commit
```
### 5. Delete a Branch
- To delete a branch locally:
```bash
    git branch -d <branch-name>
```

- To force delete a branch locally:
```bash
    git branch -D <branch-name>
```

- To delete a branch remotely:
```bash
    git push origin --delete <branch-name>
```

### 6. Revert a Commit
- To revert a specific commit by creating a new commit that undoes the changes:
```bash
    git revert <commit-hash>
```
follow the prompts to complete the revert.

### 7. Reset to a Previous Commit
- To reset your working directory to a previous commit, discarding all changes after that commit:
```bash
git reset --hard <commit-hash>
```
use the above command with caution as it will discard all changes after the specified commit

### 8. Stash Changes

- To stash your changes without committing:

```bash
git stash
```

- To list all stashed changes

```bash
git stash list
```

- To apply stashed changes:
```bash
    git stash apply
```

- To apply and drop the latest stash:
```bash
    git stash pop
```

### 9. Fetch Changes from the Remote Repository
- To fetch changes from the remote repository without merging:
```bash
    git fetch origin
```

### 10. Rebase
- To rebase your current branch onto another branch:

```bash
    git rebase <branch-name>
```












