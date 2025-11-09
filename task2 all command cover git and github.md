

## 🌟 What is Git & GitHub?

* **Git** = version control system (tool you install on your computer).
* **GitHub** = website where you can store and share your Git repositories online.

You use **Git commands** to manage code locally, and then **push** it to GitHub.

---

## 🧱 Basic Setup Commands

| Command                                            | Explanation                               | Example                                            | What Happens                             |
| -------------------------------------------------- | ----------------------------------------- | -------------------------------------------------- | ---------------------------------------- |
| `git --version`                                    | Checks Git version.                       | `git --version`                                    | Shows version, e.g. `git version 2.45.0` |
| `git config --global user.name "Your Name"`        | Sets your Git username (used in commits). | `git config --global user.name "Ali Khan"`         | Saves your name for future commits.      |
| `git config --global user.email "you@example.com"` | Sets your Git email.                      | `git config --global user.email "ali@example.com"` | Saves your email for commits.            |
| `git config --list`                                | Shows all Git configurations.             | `git config --list`                                | Displays username, email, etc.           |

---

## 📁 Repository Commands

| Command                            | Explanation                                       | Example                                                  | What Happens                           |
| ---------------------------------- | ------------------------------------------------- | -------------------------------------------------------- | -------------------------------------- |
| `git init`                         | Starts a new local Git repository.                | `git init`                                               | Creates a hidden `.git` folder.        |
| `git clone <repo-url>`             | Copies a repository from GitHub to your computer. | `git clone https://github.com/user/repo.git`             | Downloads the repo into a folder.      |
| `git remote add origin <repo-url>` | Connects local repo to GitHub repo.               | `git remote add origin https://github.com/user/repo.git` | Links your folder to GitHub.           |
| `git remote -v`                    | Shows linked GitHub URLs.                         | `git remote -v`                                          | Displays `origin` fetch and push URLs. |

---

## 📄 Working with Files

| Command                  | Explanation                           | Example                      | What Happens                                      |
| ------------------------ | ------------------------------------- | ---------------------------- | ------------------------------------------------- |
| `git status`             | Shows which files changed or are new. | `git status`                 | Lists files in red (untracked) or green (staged). |
| `git add <file>`         | Stages a specific file to commit.     | `git add index.html`         | Prepares that file for commit.                    |
| `git add .`              | Stages **all** files.                 | `git add .`                  | Adds all changes to staging area.                 |
| `git rm --cached <file>` | Unstages a file.                      | `git rm --cached index.html` | Removes it from staging area.                     |
| `git restore <file>`     | Discards changes in a file.           | `git restore index.html`     | Reverts it to last saved version.                 |

---

## 💾 Commit Commands

| Command                   | Explanation                        | Example                          | What Happens                      |
| ------------------------- | ---------------------------------- | -------------------------------- | --------------------------------- |
| `git commit -m "message"` | Saves changes with a message.      | `git commit -m "Added homepage"` | Creates a commit snapshot.        |
| `git log`                 | Shows commit history.              | `git log`                        | Lists commits with author & date. |
| `git log --oneline`       | Shorter version of log.            | `git log --oneline`              | Shows one-line commit messages.   |
| `git show <commit-id>`    | Shows what changed in that commit. | `git show 5d2f8c9`               | Displays detailed diff.           |

---

## 🔀 Branching Commands

| Command                      | Explanation                             | Example                      | What Happens                                     |
| ---------------------------- | --------------------------------------- | ---------------------------- | ------------------------------------------------ |
| `git branch`                 | Lists branches.                         | `git branch`                 | Shows current and other branches.                |
| `git branch <branch-name>`   | Creates a new branch.                   | `git branch feature-login`   | New branch created.                              |
| `git checkout <branch-name>` | Switches to a branch.                   | `git checkout feature-login` | Moves you to that branch.                        |
| `git checkout -b <branch>`   | Creates **and** switches to branch.     | `git checkout -b dev`        | Creates `dev` branch and switches.               |
| `git merge <branch>`         | Merges another branch into current one. | `git merge dev`              | Combines changes from `dev` into current branch. |
| `git branch -d <branch>`     | Deletes branch.                         | `git branch -d dev`          | Removes local branch.                            |

---

## 🌍 GitHub (Remote) Commands

| Command                    | Explanation                      | Example                                     | What Happens                              |
| -------------------------- | -------------------------------- | ------------------------------------------- | ----------------------------------------- |
| `git push origin <branch>` | Uploads commits to GitHub.       | `git push origin main`                      | Updates GitHub repo.                      |
| `git pull origin <branch>` | Downloads latest changes.        | `git pull origin main`                      | Merges latest GitHub code locally.        |
| `git fetch`                | Fetches changes without merging. | `git fetch`                                 | Updates local info, doesn’t change files. |
| `git clone <url>`          | Clone GitHub repo to local.      | `git clone https://github.com/user/app.git` | Creates local copy of repo.               |

---

## 🧹 Undo / Fix Commands

| Command               | Explanation                                 | Example               | What Happens                                |
| --------------------- | ------------------------------------------- | --------------------- | ------------------------------------------- |
| `git reset <file>`    | Unstages a file.                            | `git reset style.css` | File removed from staging area.             |
| `git reset --hard`    | Discards **all** changes.                   | `git reset --hard`    | Reverts everything to last commit.          |
| `git revert <commit>` | Undo a specific commit by making a new one. | `git revert 7f3a2c1`  | Creates new commit that undoes that change. |

---

## 🧠 Example Full Workflow

1. **Create a new repo:**

   ```bash
   git init
   ```
2. **Add files:**

   ```bash
   git add .
   ```
3. **Commit changes:**

   ```bash
   git commit -m "Initial commit"
   ```
4. **Connect to GitHub:**

   ```bash
   git remote add origin https://github.com/user/myproject.git
   ```
5. **Push to GitHub:**

   ```bash
   git push -u origin main
   ```

After running that last command — your code is now on GitHub 🎉

---
Auther: Salman Khan
