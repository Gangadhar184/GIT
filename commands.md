# Useful Git Commands for Job

## 1. **Basic Commands**

### `git init`
- **Description**: Initializes a new Git repository.
- **Use case**: You run this command when starting a new project and want to track changes with Git.
  
### `git clone <repository-url>`
- **Description**: Clone an existing repository to your local machine.
- **Use case**: Use this when you want to make a local copy of an existing project from a remote repository (e.g., GitHub).

### `git add <filename>`
- **Description**: Adds changes in the specified file(s) to the staging area.
- **Use case**: Use this to start tracking changes for the next commit.

### `git commit -m "<message>"`
- **Description**: Creates a new commit with the staged changes and a commit message.
- **Use case**: This saves your changes to the local Git repository. The message should describe what changes you made.

### `git status`
- **Description**: Shows the status of your working directory and staging area.
- **Use case**: Use this to check which files are staged, modified, or untracked.

### `git log`
- **Description**: Shows the commit history.
- **Use case**: Useful for checking past commits, including details like commit messages, authors, and dates.

## 2. **Branching and Merging**

### `git branch`
- **Description**: Lists all the branches in your repository, and highlights the currently active branch.
- **Use case**: Check which branch you're on.

### `git branch <branch-name>`
- **Description**: Creates a new branch.
- **Use case**: You create a branch to work on a feature or a fix without affecting the main codebase.

### `git checkout <branch-name>`
- **Description**: Switches to the specified branch.
- **Use case**: You use this to start working on an existing branch.

### `git checkout -b <branch-name>`
- **Description**: Creates a new branch and switches to it in one step.
- **Use case**: Commonly used when you want to quickly start a new feature or fix in a separate branch.

### `git merge <branch-name>`
- **Description**: Merges the specified branch into the current branch.
- **Use case**: You use this when you want to incorporate changes from another branch (typically after finishing a feature or bug fix).

### `git rebase <branch-name>`
- **Description**: Reapplies commits on top of another branch.
- **Use case**: Rebasing is typically used to maintain a clean commit history, especially when incorporating upstream changes into your feature branch.

## 3. **Remote Repositories**

### `git remote -v`
- **Description**: Lists the remote repositories associated with the local repository.
- **Use case**: To check the URLs for your remote (e.g., GitHub, GitLab, etc.).

### `git push <remote> <branch-name>`
- **Description**: Pushes local changes to a remote repository.
- **Use case**: You use this to upload your commits to a remote repository (e.g., pushing your branch to GitHub).

### `git pull <remote> <branch-name>`
- **Description**: Fetches changes from a remote repository and merges them into your local branch.
- **Use case**: This is used when you want to get the latest changes from a shared repository before starting work.

### `git fetch <remote>`
- **Description**: Fetches updates from a remote repository without merging them into your local branch.
- **Use case**: If you want to check for new commits in a remote repository without updating your current working branch.

### `git push origin --delete <branch-name>`
- **Description**: Deletes a branch from the remote repository.
- **Use case**: This is used when a feature branch is no longer needed and should be removed from the remote.

## 4. **Undoing Changes**

### `git reset <filename>`
- **Description**: Unstages a file that has been added to the staging area.
- **Use case**: You accidentally added the wrong file and need to remove it from the staging area.

### `git reset --hard`
- **Description**: Resets the working directory and staging area to match the most recent commit (discards all local changes).
- **Use case**: You use this when you want to completely discard changes and return to the last commit state.

### `git revert <commit-hash>`
- **Description**: Creates a new commit that undoes the changes made in a previous commit.
- **Use case**: Used when you want to undo a commit but still keep the commit history intact.

### `git checkout -- <filename>`
- **Description**: Discards changes in the working directory by restoring the file to the last committed state.
- **Use case**: You use this when you want to discard local changes in a file and revert to the version in the repository.

## 5. **Stashing Changes**

### `git stash`
- **Description**: Stashes the changes in your working directory so you can work on something else.
- **Use case**: Useful when you need to switch branches but don't want to commit your changes yet.

### `git stash apply`
- **Description**: Applies the most recent stash.
- **Use case**: After switching branches, you can apply stashed changes.

### `git stash pop`
- **Description**: Applies the most recent stash and removes it from the stash list.
- **Use case**: Similar to `git stash apply`, but removes the stash after applying it.

## 6. **Tagging**

### `git tag <tag-name>`
- **Description**: Creates a new tag at the current commit.
- **Use case**: You use tags to mark important points in your project history, like releases.

### `git push origin <tag-name>`
- **Description**: Pushes a tag to the remote repository.
- **Use case**: Tags are useful for marking versions/releases and pushing them to a remote repository.

## 7. **Viewing and Diffing**

### `git diff`
- **Description**: Shows the differences between the working directory and the staging area.
- **Use case**: Use this to see what changes have been made to files before committing.

### `git diff <commit-hash> <commit-hash>`
- **Description**: Shows the differences between two commits.
- **Use case**: Helpful for comparing the changes between two commits.

## 8. **Cleaning Up**

### `git clean -f`
- **Description**: Removes untracked files from the working directory.
- **Use case**: Use this to clean up files that are not tracked by Git.

### `git gc`
- **Description**: Cleans up unnecessary files and optimizes the local repository.
- **Use case**: Run this command when the repository gets bloated with unnecessary files and to optimize performance.

---

