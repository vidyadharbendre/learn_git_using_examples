# Installing Git for Windows

This guide will help you install Git on your Windows machine and get started with Git Bash for version control.

## Step-by-Step Installation Guide

### 1. Download Git for Windows
- Go to the official Git website: [git-scm.com](https://git-scm.com/).
- Click on the "Download" button to download the latest version of Git for Windows.

### 2. Run the Installer
- Locate the downloaded `.exe` file and double-click it to run the installer.
- You will be prompted by the User Account Control to allow the installer to make changes to your device. Click "Yes" to proceed.

### 3. Follow the Setup Wizard
- **Setup Wizard Introduction**: Click "Next".
- **Select Destination Location**: Choose the directory where you want to install Git. The default path is usually fine. Click "Next".
- **Select Components**: Choose the components you want to install. The default selection is usually sufficient. Click "Next".
- **Select Start Menu Folder**: Choose where you want the Start Menu shortcuts to be created. Click "Next".
- **Adjusting Your PATH Environment**:
  - You will be given options to adjust your PATH environment. It's recommended to select "Git from the command line and also from 3rd-party software".
  - This option allows you to use Git both in Git Bash and in Windows Command Prompt or PowerShell.
- **Choosing the SSH Executable**: Select "Use OpenSSH" (recommended). Click "Next".
- **Choosing HTTPS Transport Backend**: Select "Use the OpenSSL library" (recommended). Click "Next".
- **Configuring the Line Ending Conversions**: Select "Checkout Windows-style, commit Unix-style line endings" (recommended). Click "Next".
- **Configuring the Terminal Emulator**: Select "Use MinTTY (the default terminal of MSYS2)" (recommended). Click "Next".
- **Configuring Extra Options**: Enable any extra options you prefer. The defaults are usually fine. Click "Next".
- **Configuring Experimental Options**: Choose any experimental options you want to enable (these can usually be left unchecked). Click "Install".

### 4. Complete the Installation
- Wait for the installation to complete.
- Once the installation is complete, click "Finish" to exit the Setup Wizard. If you want to launch Git Bash immediately, you can check the box "Launch Git Bash" before clicking "Finish".

## Using Git Bash

### Open Git Bash
- After the installation, you can open Git Bash by searching for "Git Bash" in the Start menu or by right-clicking on your desktop and selecting "Git Bash Here".

### Verify Installation
- Open Git Bash and type the following command to verify that Git is installed and to check the version:
  ```bash
  git --version
