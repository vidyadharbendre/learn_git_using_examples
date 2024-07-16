# Git Practice Branch Setup

## Objective

The objective of this guide is to help you set up a practice environment using Git branches. This setup allows you to fetch the latest changes from the remote repository without pushing your practice changes back to the repository. This ensures you can practice safely without affecting the main codebase.

## Steps

### 1. Clone the Repository

If you haven't already cloned the repository, use the following command to clone it to your local machine:

```bash
git clone <repository-url>
cd <repository-directory>
```

### 2. Create a Practice Branch
Create a new branch for your practice work. This ensures that any changes you make won't affect the main branch.

```bash
git checkout -b practice
```

### 3. Fetch the Latest Changes from the Repository
Whenever you want to fetch the latest changes from the remote repository, switch to the main branch (usually main or master), fetch the latest changes, and pull them:
```bash
git checkout main
git fetch origin
git pull origin main
```

### 4. Switch Back to Your Practice Branch
After fetching the latest changes, switch back to your practice branch:
```bash
git checkout practice
```

### 5. Rebase Your Practice Branch (Optional)
If you want to keep your practice branch up to date with the latest changes from the main branch, you can rebase your practice branch:

```bash
git rebase main

```

### 6. Practice Without Pushing Changes
Now, you can practice on your practice branch. Any changes you make here won't be pushed to the remote repository unless you explicitly push them.

### 7. Ignoring Changes in Practice Branch
If you want to ensure that you don't accidentally push changes from your practice branch to the remote repository, you can use git update-index to mark the files as "assume unchanged":

```bash
git update-index --assume-unchanged <file>

```
## Summary
By following these steps, you can create a safe practice environment using Git branches. This setup allows you to always have the latest changes from the main branch without affecting your practice work.

Happy coding!