# Inventyv GitHub Practice

# GitHub Training - Basic

---

# 🚀 **Git Setup and Configuration**

## 🔹 **1. Check Git Version**
```bash
git --version
```

## 🔹 **2. Configure Git**
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

## 🔹 **3. Adding Token to Git**
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

## 🔹 **5. Verify Credentials File**
```bash
ls -a ~/
cat ~/.git-credentials
```

## 🔹 **6. Remove Stored Credentials**
```bash
rm ~/.git-credentials
```

Check which branch you are on:
```sh
git branch
```
Example Output:
```
  alpha
  beta
  dev
* main
```

---

# 🌿 **Git Branching and Merging Guide**
This repository demonstrates Git branching, merging, and workflow using multiple branches such as `main`, `beta`, `dev`, `alpha`, and `feature1`.

## 🛠 **Git Commands Used**

### ✅ 1. Creating Branches
```sh
git branch beta
git branch dev
git branch feature1
```

### ✅ 2. Switching and Committing Changes
```sh
git checkout alpha
```

### ✅ 3. Merging Branches
```sh
git checkout main
git merge feature1
```

### ✅ 4. Pushing to Remote Repository
```sh
git push origin main
```
> *Note: An origin is required to push the branch.*

## 🌍 **Branch Structure**
- **🔵 main**: The primary branch where all features get merged.
- **🟡 beta**: An experimental branch.
- **🟢 dev**: Used for development work.
- **🟠 alpha**: Contains alpha-stage features.
- **🔴 feature1**: A feature-specific branch.

## 📌 **Visual Representation**
The Git branching structure is visualized using [Learn Git Branching](https://learngitbranching.js.org/).

## 📖 **How to Use This Repo**
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

## 🔍 **Visualization using Learn Git Branching**
![Visualization](<Screenshot (178).png>)

---

# 🔄 **Pull Request Process**

### 🛡 **1. Setting Branch Protection Rules**
- Go to your repository **Settings**.
- Navigate to **Branches**.
- Set protection rules for the desired branches.
- Choose the first branch name pattern.

![Branch Protection](<Screenshot (180)-1.png>)

### 🔄 **2. Creating a Pull Request**
- Once your changes are pushed, you will see a pull request notification.

![Pull Request](<Screenshot (179)-1.png>)

### 🔀 **3. Comparing Changes**
- Compare base and feature branches (e.g., `main` and `alpha`).

![Compare Branches](<Screenshot (181)-1.png>)

### ✅ **4. Checking for Conflicts**
- If no conflicts are detected, you will see a merge option.

![Merge Status](<Screenshot (182)-1.png>)

### 🔗 **5. Merging Process**
- Review and approve the changes.
- Merge the branch into the main branch.

![Merge Process](<Screenshot (183)-1.png>)

This illustrates the entire pull request process from start to finish.

---

## 📜 **License**
Specify the license under which the project is distributed (e.g., MIT, Apache 2.0).