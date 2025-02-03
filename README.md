# inventyv-github-prac
# GitHub Training - Basic


# **Git Setup and Configuration**

## **1. Check Git Version**
```bash
git --version
```

## **2. Configure Git**
Set your user details:
```bash
git config --global user.name "ruchajogsan-inventyv"
git config --global user.email "rucha.jogsan.inventyv@gmail.com"
```
Set the default branch to `main`:
```bash
git config --global init.defaultBranch main
```
Enable color output:
```bash
git config --global color.ui auto
```
Verify the configuration:
```bash
git config --get user.name
git config --get user.email
```

## **3. Adding Token to Git**
Verify username and email:
```bash
git config --ruchajogsan-inventyv
git config --get rucha.jogsan.inventyv@gmail.com
```
Store GitHub credentials securely:
```bash
git credential approve <<'EOT'
url=https://github.com
username=<your-username>
password=<your-token>
EOT
```
Alternative one-liner:
```bash
git credential approve <<< $'url=https://github.com\nusername=<your-username>\npassword=<your-token>'
```

## **5. Verify Credentials File**
```bash
ls -a ~/
cat ~/.git-credentials
```

## **6. Remove Stored Credentials**
```bash
rm ~/.git-credentials
```

First, Clone the repository which you have created .
check status 
PS E:\github-trainning\inventyv-github-prac> git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean



check status on whichc branch you are :
PS E:\github-trainning\inventyv-github-prac> git branch
  alpha
  beta
  dev
* main
*

# Git Branching and Merging Guide

This repository demonstrates Git branching, merging, and workflow using multiple branches such as `main`, `beta`, `dev`, `alpha`, and `feature1`.

## Git Commands Used

### 1. Creating Branches
```sh
$ git branch beta
$ git branch dev
$ git branch feature1
```

### 2. Switching and Committing Changes
```sh
$ git checkout alpha

```

### 3. Merging Branches
```sh
$ git checkout main
$ git merge feature1
```

### 4. Pushing to Remote Repository
```sh
$ git push origin main
```
_Note: An origin is required to push the branch._

## Branch Structure
- **main**: The primary branch where all features get merged.
- **beta**: An experimental branch.
- **dev**: Used for development work.
- **alpha**: Contains alpha-stage features.
- **feature1**: A feature-specific branch.

## Visual Representation
The Git branching structure is visualized using [Learn Git Branching](https://learngitbranching.js.org/).

## How to Use This Repo
1. Clone the repository:
   ```sh
   git clone <repository-url>
   ```
2. Navigate to the project folder:
   ```sh
   cd <repository-folder>
   ```
3. Checkout any branch you want to work on:
   ```sh
   git checkout <branch-name>
   ```
4. Make changes and commit:
   ```sh
   git add .
   git commit -m "Your commit message"
   ```
5. Merge changes when needed:
   ```sh
   git checkout main
   git merge <branch-name>
   ```



