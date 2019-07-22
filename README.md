## Basic Commands
> git init

Starts a local working directory

> git add fileName

Adds modified and untracked files to the staging area

> git commit -m "Commit message"

Commits your changes

## Cloning Repositry

> git clone https://github.com/libgit2/libgit2

Creates a directory named libgit2, initializes a **.git** directory inside it, pulls down all the data for that repository.

## More Commands

> git diff fileName

Shows the differences between the file on your working directory and the staging area

> git show HEAD

Shows the most recently made commit

> git add fileName1 fileName2

Adds the files to the staging area together using a single git command. (Shortcut: *git add .*)

> git checkout HEAD fileName

Restores the file in your working directory to look exactly as it did when you last made a commit. Discards changes in the working directory. (often used as *git checkout -- fileName*)

> git reset HEAD fileName

Resets the file in the staging area to be the same as the HEAD commit. It does not discard file changes from the working directory, it just removes them from the staging area.

> git reset commit_SHA

Resets to a previous commit, using the first 7 characters of one of the past commit *SHAs* in your Git log. The **HEAD** commit has been reassigned. You just changed history! *HEAD goes to a previously made commit of your choice. Commits after that are no longer part of your project*