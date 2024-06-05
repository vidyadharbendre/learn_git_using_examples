
### Day-to-Day README for Basic Git Commands

```markdown
# Basic Git Commands

This guide provides a list of essential Git commands for day-to-day version control tasks.

## Step-by-Step Workflow

### 1. Check the Status of Your Repository
- Use the `git status` command to see the current status of your working directory and staging area:
  ```bash
  git status
```
### 2. Add files to the Staging Area
- To add a specific file to the staging area:
```bash
git add <file-name>
```
- To add all changes to the staging area:
```bash
git add .
```

###3. Commit Changes
- Commit the staged changes with a meaningful message:

```bash
git commit -m "Your commit message"
```
###4. Pull the Changes to the Remote Repository
- Push your committed changes to the remote repository:
```bash
git push origin <branch-name>
```

