# Creating a Public or Private Repository through Command Prompt

## Prerequisites
- Ensure Git is installed on your local machine. If not, download and install it from [git-scm.com](https://git-scm.com/).

## Step-by-Step Guide

### 1. Open Command Prompt or Terminal

### 2. Configure Git (If not already configured)
- Set your Git username and email:

```bash
  git config --global user.name "Your Name"
  git config --global user.email "your.email@example.com"
```

### 3. Create a New Directory for Your Repository
- Navigate to the directory where you want to create your new repository:

```bash
cd /path/to/your/directory
```

- Create a new directory and navigate into it:
```bash
mkdir my-new-repo
cd my-new-repo
```

### 4. Initialize a New Git Repository
- Initialize an empty Git repository:
```bash
git init
```

### 5. Create a README.md File
- Create a README.md file:

```bash
echo "# My New Repository" >> README.md

```

### 6. Add and Commit Your Changes
- Stage the README.md file:

```bash
git add README.md

```

- Commit your changes:
```bash
git commit -m "Initial commit with README"

```
### 7. Create a New Repository on GitHub (Public or Private)
- Log in to GitHub from your browser.
- Click on the + icon in the top right corner and select New repository.
- Fill in the repository details as described in the web interface guide
  above. Ensure the repository is empty (no README, .gitignore, or license).

### 8. Link Your Local Repository to GitHub
- Copy the repository URL (either HTTPS or SSH) from GitHub.
- Add the remote URL to your local repository:

```bash
git remote add origin https://github.com/yourusername/my-new-repo.git

```

- Push your local commits to the remote repository:
```bash
git push -u origin master

```

### Example
- Here’s a summary of the commands used:

```bash

cd /path/to/your/directory
mkdir my-new-repo
cd my-new-repo
git init
echo "# My New Repository" >> README.md
git add README.md
git commit -m "Initial commit with README"
git remote add origin https://github.com/yourusername/my-new-repo.git
git push -u origin master

```
