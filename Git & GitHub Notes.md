# An Introduction to Git and GitHub by Brian Yu
### _Sameera Rajaratne_

__What is Git?__
1. Keep track of changes to code.
2. Synchronizes code between different people.
3. Test changes to code without losing the original.
4. Revert back to old versions of code.

__git clone__
- makes a copy of a repository
- stores it on your computer
- a "fork" creates your own copy of someone else's repository

_Usage:_ git clone <url>

__git add__
- adds a file to "staging area"
- tells git to include the file in the next revision to the repository
- git add * adds all changed files

_Usage:_ git add <file_name>

__git commit__
- saves the changes to repository as a new revision (a "commit")
- records a message. A message is usually some summary of the changes you made in this particular change.
- git commit -am "message" adds and commits in same step

_Usage:_ git commit -m "message"

__git status__
- shows current status of repository

_Usage:_ git status

__git push__
- sends committed changes to remote repository (e.g. to GitHub)
- more explicitly, could write git push origin master

_Usage:_ git push

__git pull__
- retrieves changes from remote repository

_Usage:_ git pull

__Merge Conflicts__
- when two different commits can't be automatically merged
- needs to be resolved

__git log__
- shows a history of commits and messages
- make sure you use good commit messages if you are going to use Git

_Usage:_ git log

__git reset__
- reverts code back to a previous commit / revision. You lose all recent changes.
- git reset --hard <commit> reverts code back to a previous commit
- git reset --hard origin/master reverts code back to remote repository main

_Usage:_
- git reset --hard <commit#>
- git reset --hard origin/master

__Branching__
1. Branch is a version of the repository.
2. Each branch has its own commit history and current version.

__git branch__
- shows all branches of code
- create a branch with git branch <branch_name>
- switch to ("checkout") a new branch with git checkout <branch_name>
- delete a branch with git branch -D <branch_name>

_Usage:_
- git branch: shows all branches of code
- git branch <branch_name>: create new branch
- git checkout <branch_name>: switch to branch
- git checkout -b <branch_name>: create and switch to a new branch
- git branch -D <branch_name>: delete branch branch_name

__git merge__
- merge two different branches together
- git merge <branch_name> merges the branch branch_name with current branch

_Usage:_ git merge <branch_name>
