# Git offers a suite of collaboration tools to make working with others on a project easier.

## Git Cloning and Remotes

> git clone remote_location clone_name

**remote_location** tells Git where to go to find the remote. This could be a web address, or a filepath (*/Users/teachers/Documents/some-remote*)

**clone_name** is the name you give to the directory in which Git will clone the repository

> git remote -v

Lists the name of the remote, origin, as well as its location.

> git fetch

Brings those changes from the remote onto a remote branch (*origin/master*) in your Local Repository. It **does not merge** changes from the remote into your local *master* branch. To integrate *origin/master* into your local *master* branch: *git merge origin/master*

> git push origin your_branch_name

Pushes your local branch up to the **origin** remote.