# Cloning an Existing Repository

This guide will help you clone an existing GitHub repository to your local machine.

## Step-by-Step Guide

### 1. Navigate to the GitHub Repository
- Go to the GitHub page of the repository you want to clone.

### 2. Copy the Repository URL
- Click on the green "Code" button.
- Choose either the SSH or HTTPS tab.
- Copy the URL provided.

### 3. Open Git Bash
- Open Git Bash by searching for "Git Bash" in the Start menu or by right-clicking on your desktop and selecting "Git Bash Here".

### 4. Navigate to Your Desired Directory
- In Git Bash, navigate to the directory where you want to clone the repository:
```bash
    cd path/to/your/directory
```

### 5. Clone the Repository
- In Git Bash, type 'git clone' followed by the URL that you copied from GitHub:
```bash
    path/to/your/directory>git clone https://github.com/username/repository.git
```
- or if you chose the SSH URL:
```bash
    git clone git@github.com:username/repository.git
```

### 6. Navigate to the Cloned Repository
- Change directory to the newly cloned repository:
```bash
cd repository
```

### 7. Verify the cloning 
- To verify that the repository was cloned successfully, you can list the contents of the directory:
```bash
ls -la
```
- You should see all the files and directories from the remote repository in your local directory.


