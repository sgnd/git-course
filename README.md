# Git CheatSheet

This cheatsheet provides a list of the most commonly used Git commands, grouped by category. It's a quick reference for developers who are already familiar with Git, but need a reminder of the syntax and options for specific commands.

## Common commands

- `git clone <repository>` - creates a local copy of a remote repository
- `git init` - creates a new Git repository in the current directory
- `git add <file>` - stages a file for commit
- `git commit -m "<message>"` - commits the staged changes with a message
- `git push` - pushes the committed changes to a remote repository
- `git pull` - fetches and merges changes from a remote repository
- `git branch <branch>` - creates a new branch
- `git checkout <branch>` - switches to a different branch
- `git merge <branch>` - merges a branch into the current branch
- `git status` - displays the current state of the repository

## Branching and merging

- `git branch -d <branch>` - deletes a local branch
- `git push <remote> --delete <branch>` - deletes a remote branch
- `git cherry-pick <commit>` - applies the changes from a specific commit to the current branch
- `git rebase <branch>` - reapplies commits from the current branch on top of another branch
- `git cherry-pick --abort` - aborts the cherry-pick operation
- `git rebase --abort` - aborts the rebase operation

## Stashing and cleaning

- `git stash` - temporarily saves changes that have not been committed
- `git stash pop` - restores the changes saved with `git stash` and removes the stash
- `git stash apply` - restores the changes saved with `git stash`, but leaves the stash in place
- `git stash drop` - discards the latest stash
- `git stash list` - displays a list of stashes
- `git stash clear` - removes all stashes
- `git stash branch <branch>` - creates a new branch and restores the changes saved with `git stash`
- `git clean <args>` - removes untracked files and directories from the working tree

## History and diffs

- `git log` - displays a log of commits on the current branch
- `git diff` - shows the changes made in the uncommitted files
- `git blame <file>` - shows the commit and the name of the person who last modified each line of a file
- `git show <commit>` - displays information about a specific commit
- `git bisect` - performs a binary search through the commit history to find a specific change
- `git bisect reset` - exits the binary search
- `git rev-list` - lists commit objects in reverse chronological order
- `git rev-list --all` - lists all commit objects
- `git rev-list --branches` - lists commit objects reachable from any branch
- `git rev-list --remotes` - lists commit objects reachable from any remote branch
- `git rev-list --tags` - lists commit objects reachable from any tag
- `git rev-list --stdin` - reads commit objects from the standard input
- `git rev-list --quiet` - suppresses the default output of `git rev-list`

## Remote repositories

- `git fetch` - downloads objects and references from a remote repository
- `git fetch --all` - fetches updates from all remote repositories
- `git fetch --prune` - prunes local branches that have been deleted on the remote
- `git push` - pushes the committed changes to a remote repository
- `git push --tags` - pushes all tags to the remote repository
- `git ls-remote` - displays references in a remote repository
- `git remote prune <remote>` - removes local branches that have been deleted on the remote
- `git remote add <remote> <url>` - adds a new remote repository
- `git remote set-url <remote> <url>` - sets the URL for a remote repository
- `git remote rename <old> <new>` - renames a remote repository
- `git remote show <remote>` - displays information about a remote repository
- `git remote` - lists the remote repositories for the current repository

## Tags

- `git tag <tag>` - adds a tag to the current commit
- `git tag -d <tag>` - deletes a local tag
- `git push <remote> --delete <tag>` - deletes a remote tag

## Miscellaneous

- `git log --oneline` - displays a condensed summary of the commit history
- `git log --decorate` - displays references in the commit log
- `git log --graph` - displays a graphical representation of the commit history
- `git log --follow <file>` - displays the commit history for a file, including renames
- `git shortlog` - displays a summary of commits by author
- `git describe <ref>` - displays a human-readable description of a commit
- `git reset <file>` - removes a file from the staging area
- `git mv <old> <new>` - renames a file
- `git rm <file>` - removes a file from the repository and the filesystem
- `git show-ref` - lists references in the local repository
- `git for-each-ref` - performs an action on each reference
- `git symbolic-ref <ref> <name>` - creates a symbolic reference
- `git symbolic-ref --short <ref>` - expands a symbolic reference to its shorthand name
- `git for-each-ref --format <format>` - customizes the output of `git for-each-ref`
