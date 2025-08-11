# Git

Git is a distributed version control system that tracks changes, manages code history, and enables multiple developers to work simultaneously through branching and merging.

---

### Configuration

| Command                                 | Description                      |
| --------------------------------------- | -------------------------------- |
| git config --global user.name [name]    | Sets the global user name        |
| git config --global user.email [email]  | Sets the global user email       |
| git config --list                       | Lists all current configurations |

---

### Repository

| Command          | Description                        |
| ---------------- | ---------------------------------- |
| git init         | Creates a new local Git repository |
| git clone [url]  | Clones a remote repository         |

---

### Status and Logs

| Command           | Description                                            |
| ----------------- | ------------------------------------------------------ |
| git status        | Shows the current repository status                    |
| git log           | Displays the commit history                            |
| git log --oneline | Shows a condensed commit history (one line per commit) |
| git show [hash]   | Shows details of a specific commit                     |

---

### Staging and Commit

| Command                  | Description                          |
| ------------------------ | ------------------------------------ |
| git add [file]           | Adds file(s) to the staging area     |
| git add .                | Adds all changes to the staging area |
| git commit -m [message]  | Creates a commit with a message      |
| git reset [file]         | Removes a file from the staging area |

---

### Branches

| Command                 | Description                                     |
| ----------------------- | ----------------------------------------------- |
| git branch              | Lists local branches                            |
| git branch [name]       | Creates a new branch                            |
| git checkout [name]     | Switches to the specified branch                |
| git checkout -b [name]  | Creates and switches to a new branch            |
| git merge [branch]      | Merges the specified branch into current branch |
| git branch -d [name]    | Deletes a local branch                          |

---

### Remote

| Command                      | Description                                        |
| ---------------------------- | -------------------------------------------------- |
| git remote -v                | Shows configured remote repositories               |
| git remote add origin [url]  | Adds a remote repository                           |
| git push -u origin [branch]  | Pushes branch to remote and sets upstream tracking |
| git push                     | Pushes commits to the remote repository            |
| git pull                     | Fetches changes from remote and merges             |

---

### Reset, Revert, and Stash

| Command                  | Description                                            |
| ------------------------ | ------------------------------------------------------ |
| git reset --hard [hash]  | Resets repo to a specific commit (loses local changes) |
| git revert [hash]        | Reverts a commit by creating a new commit              |
| git stash                | Temporarily stores local changes                       |
| git stash pop            | Reapplies the stored changes                           |

---

### Tags

| Command                | Description                     |
| ---------------------- | ------------------------------- |
| git tag                | Lists all tags                  |
| git tag [name]         | Creates a new tag               |
| git push origin [tag]  | Pushes a specific tag to remote |

---