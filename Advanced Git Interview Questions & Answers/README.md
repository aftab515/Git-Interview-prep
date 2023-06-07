# Advance Git Interview Questions & Answers

## Written by <https://github.com/aftab515>

### 96. Explain the different points when a merge can enter a conflicted stage?

There are two stages when a merge can enter a conflicted stage.

- Starting the merge process

If there are changes in the working directory of the stage area in the current project, the merge will fail to start. In this case, conflicts happen due to pending changes that need to be stabilized using different Git commands.

- During the merge process

The failure during the merge process indicates that there’s a conflict between the local branch and the branch being merged. In this case, Git resolves as much as possible, but some things have to be fixed manually in the conflicted files.

### 97. What has to be run to squash the last N commits into a single commit?

In Git, squashing commits means combining two or more commits into one.

Use the below command to write a new commit message from the beginning.

git reset -soft HEAD~N &&git commit

But, if you want to edit a new commit message and add the existing commit messages, then you must extract the messages and pass them to Git commit.

The below command will help you achieve this:

git reset -soft HEAD~N &&git commit -edit -m“$(git log -format=%B -reverse .HEAD@{N})”

### 98. What is the difference between fork, branch, and clone?

| Fork | Branch | Clone |
| -------- | -------- | -------- |
| The fork is the process when a copy of the repository is made. It's usually experimentation in the project without affecting the original project. They’re used to advise changes or take inspiration from someone else’s project.   | Git branches refer to individual projects within a git repository. If there are several branches in a repository, then each branch can have entirely different files and folders.   | Git clone refers to creating a clone or a copy of an existing git repository in a new directory. Cloning automatically creates a connection that points back to the original repository, which makes it very easy to interact with the central repository.   |

### 99. How is Git merge different from Git rebase?

Git merge is used to incorporate new commits into your feature branch.

<img src="./images/git merge.png" alt="Example Image" width="300" height="200">

- Git merge creates an extra merge commit every time you need to incorporate changes.
- It pollutes your feature branch history.

As an alternative to merging, you can rebase the feature branch into master.

<img src="./images/rebase & merge .jpg" alt="Example Image" width="300" height="200">

- Git rebase Incorporates all the new commits in the master branch.
- It rewrites the project history by creating brand new commits for each commit in the original branch

### 100. What is the command used to fix a broken commit?

To fix a broken commit in Git, you may use the “git commit --amend” command, which helps you combine the staged changes with the previous commits instead of creating an entirely new commit.

### 101. How do you recover a deleted branch that was not merged?

To recover a deleted branch, first, you can use the git reflog command. It will list the local recorded logs for all the references. Then, you can identify the history stamp and recover it using the git checkout command.

### 102. What is git stash drop?

The Git stash drop command is used to remove a particular stash. If there’s a stash you're no longer using or you want to remove a specific item of stash from the list, you can use the stash commands.

Let’s say you want to delete an item named stash@{abc}; you can use the command:

git stash drop stash@{abc}.

### 103. What’s the difference between reverting and resetting?

| Reverting | Resetting |
| -------- | -------- |
| The revert command in Git is used to create a new commit that undoes the changes made in the previous commit. When you use this command, a new history is added to the project; the existing history is not modified.   | Git reset is a command that is used to undo the local changes that have been made to a Git repository. Git reset operates on the following: commit history, the staging index, and the working directory.   |

### 104. How can you discover if a branch has already been merged or not?

There are two commands to determine these two different things.

git branch --merged - Returns the list of branches that have been merged into the current branch.

git branch --no-merged - Returns the list of branches that have not been merged.

### 105. What is “git cherry-pick”?

The command git cherry-pick enables you to pick up commits from a branch within a repository and apply it to another branch. This command is useful to undo changes when any commit is accidentally made to the wrong branch. Then, you can switch to the correct branch and use this command to cherry-pick the commit.
