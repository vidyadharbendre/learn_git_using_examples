# Cloning a Private GitHub Repository using a Personal Access Token (PAT)

To clone a private GitHub repository using the command prompt, you need to use a Personal Access Token (PAT) for authentication. Here are the steps:

### 1. Generate a Personal Access Token (PAT)

1. **Log in to GitHub.**

2. **Go to Settings:**
   - Click on your profile picture in the upper-right corner.
   - Select "Settings" from the dropdown menu.

3. **Access Developer Settings:**
   - In the left sidebar, click "Developer settings."

4. **Generate a New Token:**
   - Click "Personal access tokens."
   - Click "Tokens (classic)" or "Fine-grained tokens" depending on what your GitHub UI shows.
   - Click "Generate new token" or "Generate new token (classic)."

5. **Configure the Token:**
   - Give your token a descriptive name.
   - Select the scopes or permissions you need. At a minimum, you’ll need the `repo` scope to access repositories.
   - Click "Generate token."

6. **Copy the Token:**
   - **Important:** Copy the token now, as you won’t be able to see it again.

### 2. Clone the Repository Using the PAT

1. **Open your terminal or command prompt.**

2. **Clone the repository using HTTPS and the PAT:**
```bash
   git clone https://<your-username>:<your-token>@github.com/<your-username>/<repository-name>.git
```

Replace <your-username> with your GitHub username, <your-token> with the generated PAT, and <repository-name> with the name of your repository.

### 3. Configure Git to Store Your Credentials
To avoid entering your PAT each time, you can configure Git to store your credentials securely.

Configure Git to Use the Credential Helper:

## For macOS

```bash
git config --global credential.helper osxkeychain

```

## For Windows

```bash
git config --global credential.helper wincred

```
## For Liunx

```bash
git config --global credential.helper cache

```

or for longer-term caching:

```bash
git config --global credential.helper 'cache --timeout=3600'

```