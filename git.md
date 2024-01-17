# Git Cheat Sheet

A cheat sheet for Git commands.

#

## Table of Contents

- [Installation](#installation)
- [Setup / Configuration](#setup--configuration-source)
- [Basics](#basics)

  - [Initialize a Repository](#initialize-a-repository)
  - [Stage and Snapshot](#stage-and-snapshot)
  - [Commit Update](#commit-update)
  - [Branches](#branches)
  - [Log and Show](#log-and-show)
  - [Stash](#stash)
  - [Tags](#tags)

- [Tutorials](#tutorials)

  - [Adding locally hosted code to GitHub](#adding-locally-hosted-code-to-github-source)
  - [Push existing repository to new remote](#push-existing-repository-to-new-remote)
  - [Deploy React app to Github pages](#deploy-react-app-to-github-pages-source)

- [Other](#other)
  - [.gitignore](#gitignore)
  - [Remove from remote repository](#remove-from-remote-repository)
  - [Remove file history from header](#remove-file-history-from-header)
  - [set new remote url](#set-new-remote-url)

#

## Installation

| Commands                               | Description                           | Link                               |
| -------------------------------------- | ------------------------------------- | ---------------------------------- |
| Git for Windows stand-alone installer. | Install via installer                 | https://git-scm.com/download/win   |
| `$ brew install git`                   | Install Git with Homebrew on Mac OS   | https://git-scm.com/download/mac   |
| `$ sudo port selfupdate`               | Install Git with MacPorts on Mac OS   |                                    |
| `$ sudo apt-get install git`           | Install Command for Linux             | https://git-scm.com/download/linux |
| `$ git –version`                       | Shows the current version of your Git |                                    |

#

## Setup / Configuration [source](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup)

```bash
git config --global user.name "Your Name"               # Set your username globally.
git config --global --unset-all user.name               # Remove the global username.
git config --global user.email "youremail@example.com"  # Set your email globally.
git config --global --unset-all user.email              # Remove the global email.
git config --global user.name                           # Check your username.
git config --global user.email                          # Check your email.
git config --global --edit                              # Open the global configuration file in a text editor for manual editing.
git config --list                                       # List all global configuration settings.
git config --global color.ui true                       # Enables helpful colorization of command line output.
git config --global core.editor "code --wait"           # Set Visual Studio Code as your default editor.
git config --global core.editor "nano -w"               # Set nano as your default editor.
git config --global core.editor "vim"                   # Set vim as your default editor.
git config --global core.editor "subl -n -w"            # Set sublime as your default editor.
git config --global core.editor "notepad++ -multiInst"  # Set notepad++ as your default editor.
```

#

## Basics [source](https://git-scm.com/book/en/v2/Git-Basics-Getting-a-Git-Repository)

### Initialize a Repository

```bash
git init                   # Initialize a local Git repository in your working directory.
git init -b <branch>       # Initialize a local Git repository in your working directory with a branch.
git init <directory>       # Create an empty Git repository in the specified directory.
git clone <url>            # Clone a remote repository into a new directory.
git clone <url> <directory> # Clone a remote repository into a new directory with a specific name.
git clone --branch <branch> <repository_url>                  # Clone a specific branch from a remote repository.
git clone --branch <branch> <repository_url> <directory> # Clone a specific branch from a remote repository into a new directory.
```

#

### Stage and Snapshot

```bash
git status                   # Show modified files in the working directory, staged for your next commit.
git status --ignored         # Show ignored files in the working directory in addition to the regular status output.
git add <file>               # Add a file as it looks now to your next commit (stage).
git add .                    # Add all files as they look now to your next commit (stage).
git add -A                   # Add all files as they look now to your next commit (stage).
git add --all                # Add all files as they look now to your next commit (stage).
git reset <file>             # Unstage a file while retaining the changes in the working directory.
git diff                     # Diff of what is changed but not staged.
git diff <commit1> <commit2> # Displays the differences between two commits.
git diff --staged            # Diff of what is staged but not yet committed.
git diff --cached            # Diff of what is staged but not yet committed.
git diff HEAD                # Display the difference between the current directory and the last commit.
git commit -m "<message>"    # Commit your staged content as a new commit snapshot.
git commit -a                # Commit any files you've added with git add and also commit any files you've changed since then.
git commit -am "<message>"   # Commit any files you've added with git add and also commit any files you've changed since then.
git notes add                # Creates a new note and associates it with an object (commit, tag, etc.).
git restore <file>           # Restores the file in the working directory to its state in the last commit.
git reset <commit>           # Resetting the staging area and the working directory to the state of the specified commit.
git reset --soft <commit>    # Preserving the changes in the staging area and the working directory.
git reset --hard <commit>    # Effectively resetting the repository to the specified commit.
git rm <file>                # Removes a file from both the working directory and the repository, staging the deletion.
git mv                       # Moves or renames a file or directory in your Git repository.
```

#### Commit Update

```bash
git commit -m "feat: message"     # indicate a new feature commit in the repository.
git commit -m "fix: message"      # fix the bugs in codebases.
git commit -m "chore: message"    # show routine tasks or maintenance.
git commit -m "refactor: message" # change the code base and improve the structure.
git commit -m "docs: message"     # change the documentation.
git commit -m "style: message"    # change the styling and formatting of the codebase.
git commit -m "test: message"     # indicate test-related changes.
git commit -m "perf: message"     # indicate performance-related changes.
git commit -m "ci: message"       # indicate continuous integration (CI) system-related changes.
git commit -m "build: message"    # indicate changes related to the build process.
git commit -m "revert: message"   # indicate changes related to reverting a previous commit.
git commit -m "merge: message"    # indicate changes related to merging branches.
git commit -m "release: message"  # indicate changes related to releasing a new version.
git commit -m "security: message" # indicate security-related changes.
git commit -m "hotfix: message"   # indicate hotfix-related changes.
```

#

### Branching and Merging

```bash
git branch                   # List your branches. a * will appear next to the currently active branch.
git branch -a                # List all branches (local and remote).
git branch -r                # List remote branches.
git branch <branch>          # Create a new branch.
git branch -m <oldname> <newname> # Rename a branch.
git branch -m <newname>      # Rename the current branch.
git branch -d <branch>       # Delete a branch.
git branch -D <branch>       # Force delete a branch.
git checkout <branch>        # Switch to a branch.
git checkout -b <branch>     # Create a new branch and switch to it.
git merge <branch>           # Merge a branch into the active branch.
git switch <branch>          # Switch to a branch.
git switch -c <branch>       # Create a new branch and switch to it.
```

#### Stash

```bash
git stash                    # Stash the changes in the working directory away (allowing you to switch branches).
git stash list               # List all stashed changesets.
git stash pop                # Apply the stashed changes to your working directory.
git stash drop               # Discard the most recently stashed changeset.
git stash clear              # Discard all stashed changesets.
```

#### Tags

```bash
git tag                      # List all tags.
git tag <tagname>            # Create a new tag.
git tag <tagname> <commit>   # Create a new tag for a specific commit.
git tag -d <tagname>         # Delete a tag.
git push origin <tagname>    # Push a tag to your remote repository.
git push origin --tags       # Push all tags to your remote repository.
git checkout <tagname>       # Checkout a tag (creates a detached head).
```

### Remote Repositories

```bash
git fetch                    # Fetch changes from the remote repository.
git fetch <remote>           # Fetch changes from the specified remote repository.
git fetch -prune             # Fetch changes from the remote repository and remove any remote-tracking references that no longer exist on the remote.
git pull                     # Fetch and merge changes from the remote repository.
git pull <remote>            # Fetch and merge changes from the specified remote repository.
git pull --rebase            # Fetch and rebase on the current branch.
git push                     # Pushes local commits to the remote repository.
git push <remote>            # Pushes local commits to the specified remote repository.
git push -u <remote> <branch> # Pushes local commits to the specified branch of the remote repository.
git puss -all                # Pushes all local branches to the remote repository.
git remote                   # List all currently configured remote repositories.
git remote add <name> <url> # Add a new remote repository.
git remote -v                # List all currently configured remotes.

```

### Inspect and Compare

```bash
git log                      # Show the commit history for the currently active branch.
git log <branch>             # Show the commit history for the specified branch.
git log --oneline            # Show the commit history for the currently active branch in one line.
git log --oneline <branch>   # Show the commit history for the specified branch in one line.
git log --stat               # Show the commit history for the currently active branch and list the files that were changed.
git log --stat <branch>      # Show the commit history for the specified branch and list the files that were changed.
git log -p                   # Show the commit history for the currently active branch and list the content changes.
git log -p <branch>          # Show the commit history for the specified branch and list the content changes.
git log --graph              # Show the commit history for the currently active branch in a nice graph.
git log --graph <branch>     # Show the commit history for the specified branch in a nice graph.
git show                     # Show the metadata and content changes of the last commit.
git show <commit>            # Show the metadata and content changes of the specified commit.
git show <commit>:<filename> # Show the content changes of the specified commit and filename.
git log –follow <file>       # Show the commits that changed file, even across renames.
git show HEAD                # Show the metadata and content changes of the last commit.
git show HEAD~3              # Show the metadata and content changes of the 3rd last commit.
git show HEAD~3:<filename>   # Show the content changes of the 3rd last commit for the specified filename.
```

Managing History

```bash
git revert <commit>          # Create a new commit that undoes all of the changes made in <commit>, then apply it to the current branch.
git revert HEAD              # Create a new commit that undoes all of the changes made in the last commit, then apply it to the current branch.
git revert --no-commit <commit> # Undoes the changes introduced by the specified commit, but does not create a new commit.
git rebase <branch>          # Reapplies commits on the current branch onto the tip of the specified branch.
```

#

## Tutorials

### Adding locally hosted code to GitHub [source](https://docs.github.com/en/migrations/importing-source-code/using-the-command-line-to-import-source-code/adding-locally-hosted-code-to-github)

1. Initialize the local directory as a Git repository

```bash
git init -b <branch>
```

2. Add the files in your new local repository

```bash
git add .
```

3. Commit

```bash
git commit -m "First commit"
```

4. Add the URL for the remote repository

```bash
git remote add origin REMOTE-URL
```

5. Verify that you set the remote URL correctly

```bash
git remote -v
```

6. Push the created branch to github

```bash
git push origin <branch>
```

7. Set the remote as upstream branch

```bash
git push --set-upstream origin <branch>
```

#

### Push existing repository to new remote

1. Create new branch if needed

```bash
git checkout -b <branch>
```

2. Rename origin upstream

```bash
git remote rename origin upstream
```

3. Add New repository URL

```bash
git remote add origin REMOTE-URL
```

4. Push a branch to github

```bash
git push origin <branch>
```

7. Set the remote as upstream branch

```bash
git push --set-upstream origin <branch>
```

#

### Deploy React app to Github pages [source](https://www.freecodecamp.org/news/deploy-a-react-app-to-github-pages/)

1. Add locally hosted code to GitHub (see above)

2. install gh-pages packages

```bash
npm install gh-pages --save-dev https://www.npmjs.com/package/gh-pages
```

3. Add keys to script inside package.json

```bash
"predeploy": "npm run build",
"deploy": "gh-pages -d build",
```

4. Add homepage field to top of package.json

```bash
"homepage": "URL",
```

5. Deploy

```bash
npm run deploy
```

#

## Other

### [.gitignore](https://www.freecodecamp.org/news/gitignore-file-how-to-ignore-files-and-folders-in-git/#introduction)

1. create a .gitignore file

```bash
touch .gitignore
```

2. Add all files and folders you want to ignore to the .gitignore file

#

### Remove from remote repository

1. Add to .gitignore
2. Remove from Git Tracking

```bash
git rm -r --cached path_to_your_folder/
```

#

### Remove file history from header

git filter-branch --index-filter 'git rm -r --cached --ignore-unmatch <DIR/FILE>' HEAD

### set new remote url

```bash
git remote set-url origin {new url}
```
