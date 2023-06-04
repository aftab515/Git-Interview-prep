# Intermediate Git Interview Questions

### 17. What does the git push command do?

The Git push command is used to push the content in a local repository to a remote repository. After a local repository has been modified, a push is executed to share the modifications with remote team members.

<img src="" alt="Example Image" width="300" height="200">   

### 18. Difference between git fetch and git pull.

| Git Fetch | Git Pull |
|----------|----------|
| The Git fetch command only downloads new data from a remote repository.    | Git pull updates the current HEAD branch with the latest changes from the remote server.    |
| It does not integrate any of these new data into your working files.    | Downloads new data and integrate it with the current working files.    |
| Command - git fetch origin    | Tries to merge remote changes with your local ones.   |
| git fetch --all    | Command - git pull origin master    |

### 19. GitHub, GitLab and Bitbucket are examples of git repository _______ function?

Hosting. All the three are services for hosting Git repositories

### 20. What do you understand about the Git merge conflict?

A Git merge conflict is an event that occurs when Git is unable to resolve the differences in code between the two commits automatically. 

Git is capable of automatically merging the changes only if the commits are on different lines or branches.

<img src="" alt="Example Image" width="300" height="200">

### 21. How do you resolve conflicts in Git?

Here are the steps that will help you resolve conflicts in Git:

- Identify the files responsible for the conflicts.
- Implement the desired changes to the files.
- Add the files using the git add command.
- The last step is to commit the changes in the file with the help of the git commit command.

### 22. What is the functionality of git ls-tree?

The git ls-tree command is used to list the contents of a tree object.

### 23. What is the process to revert a commit that has already been pushed and made public?

There are two processes through which you can revert a commit:

- Remove or fix the bad file in a new commit and push it to the remote repository. Then commit it to the remote repository using:

git commit –m “commit message”

- Create a new commit to undo all the changes that were made in the bad commit. Use the following command:

git revert <commit id>

### 24. How is a bare repository different from the standard way of initializing a Git repository?

| Standard way | Bare way |
|----------|----------|
| You create a working directory with the git init command.    | Does not contain any working or checked out copy of source files.    |
| A .git subfolder is created with all the git-related change history.    | Bare repositories store git revision history in the root folder of your repository instead of the .git subfolder.    |

### 25. What does git clone do?

Git clone allows you to create a local copy of the remote GitHub repository. Once you clone a repo, you can make edits locally in your system rather than directly in the source files of the remote repo

### 26. What is Git stash?

Let’s say you're a developer and you want to switch branches to work on something else. The issue is you don’t want to make commits in uncompleted work, so you just want to get back to this point later. The solution here is the Git stash.

Git stash takes your modified tracked files and saves it on a stack of unfinished changes that you can reapply at any time. To go back to the work you can use the stash pop.

### 27. What does the git reset --mixed and git merge --abort commands do?

git reset --mixed is used to undo changes made in the working directory and staging area.

git merge --abort helps stop the merge process and return back to the state before the merging began.

### 28. What do you understand about the Staging area in Git?

The Staging Area in Git is when it starts to track and save the changes that occur in files. These saved changes reflect in the .git directory. Staging is an intermediate area that helps to format and review commits before their completion.

### 29. What is Git Bisect and how do you use it?

The Git Bisect command performs a binary search to detect the commit which introduced a bug or regression in the project’s history.

Syntax: git bisect <subcommand> <options>

### 30. How do you find a list of files that has been changed in a particular commit?

The command to get a list of files that has been changed in a particular commit is:

git diff-tree –r {commit hash}

-r flag allows the command to list individual files
commit hash lists all the files that were changed or added in the commit.

### 31. What is the use of the git config command?

The git config command is used to set git configuration values on a global or local level. It alters the configuration options in your git installation. It is generally used to set your Git email, editor, and any aliases you want to use with the git command.

### 32. What is the functionality of git clean command?

The git clean command removes the untracked files from the working directory.

### 33. What is SubGit and why is it used?

SubGit is a tool that is used to migrate SVN to Git. It transforms the SVN repositories to Git and allows you to work on both systems concurrently. It auto-syncs the SVN with Git.

### 34. If you recover a deleted branch, what work is restored?

The files that were stashed and saved in the stashed index can be recovered. The files that were untracked will be lost. Hence, it's always a good idea to stage and commit your work or stash them. 

### 35. Explain these commands one by one– git status, git log, git diff, git revert <commit>,  git reset <file>.

Git status - It shows the current status of the working directory and the staging area.
Git revert<commit> -  It is used for undoing changes to a repository's commit history.
Git log- It is a key tool for reviewing and reading the history of everything that happens to a repository.
Git diff- It is a multi-purpose Git command that performs a diff function on Git data sources when executed.
Git reset<file>- it is used to unstage a file.
### 36. What exactly is tagging in Git?

Tagging enables developers to mark all significant checkpoints as their projects progress.

### 37. What exactly is forking in Git?

It is a repository duplicate and forking allows one to experiment with changes without being concerned about the original project.

### 38. How to change any older commit messages?

You can change the most recent commit message with the git commit —amend command.

### 39. How to handle huge binary files in Git?

Git LFS is a Git extension for dealing with large and binary files in a separate Git repository.

### 40. Name a few GIT tools.

Git comes with a few built-in tools like Git Bash and Git GUI.

### 41. Will you make a new commit or amend an existing one?

The git commit —amend command allows you to easily modify the most recent commit.

### 42. What do you mean by branching strategy?

It is employed by a software development team while writing and managing code with a version control system.

### 43. Difference between head, working tree, and index.

They are all names for various branches. Even Though a single git repository can track an arbitrary number of branches, the working tree is only associated with one of them, and HEAD points to that branch.

### 44. Is there a git GUI client available for Linux?

Git includes built-in GUI tools for committing (git-gui) and browsing (gitk), but there are a number of third-party tools available for users seeking platform-specific experience.

### 45. What is the benefit of a version control system?

Version control enables software teams to maintain efficiency and agility while the team grows by adding more developers

### 46. What do you mean by git instaweb?

It is a script used to set up a temporary instance of Gitweb.

### 47. What exactly is the forking workflow?

Forking is a git clone operation that is performed on a server copy of a project's repository.

### 48. Mention benefits of forking workflow.

Contributions can be integrated without everyone trying to push to a single central repository.

### 49. What is the Gitflow workflow?

The Gitflow Workflow specifies a strict branching model centered on the project release.

### 50. What does the commit object contain?

The commit object contains a tree of blob objects and other tree objects that represent the project revision's directory structure.

### 51. Write the syntax of rebasing in git.

Syntax is as follows: $git rebase <branch name>

### 52. What are Git Hooks?

They are scripts that are executed automatically whenever a specific event occurs in a Git repository.

### 53. What is Git stash vs Git stash pop?

Git stash pop removes the (topmost, by default) stash when applied, whereas git stash apply keeps it in the stash list for future use.

### 54. Explain git reflog This command is used by Git to record changes made to the branches' tips?

The git reflog command is used to display a log of reference changes in Git, specifically the changes made to the tips of branches. It stands for "reference log" and provides a history of all the recent updates to the branch pointers, including commits, merges, rebases, branch creations, and deletions.

Here are a few key points about git reflog:

- Reference Changes: The command shows a chronological list of reference changes, including branch head movements, commits, and other operations that affect the branch pointers.

- Local Repository: The git reflog command operates locally and shows the reference log specific to your local repository. It does not interact with remote repositories.

- Temporary History: The reference log is a temporary history and is not shared with collaborators or pushed to remote repositories by default. It is primarily intended for local repository management and troubleshooting purposes.

- Useful for Recovery: git reflog is particularly useful for recovering lost commits or branches. If you accidentally delete a branch or perform a reset, the reference log can help you identify the commit or branch pointer before the operation and restore it.

- Reflog Entries: Each entry in the reference log typically includes a commit hash, the branch it points to, the operation performed, and the original position of the branch pointer before the change.

#### Conclusion:

By using git reflog, you can review the recent changes made to branch tips, track down lost commits or branches, and potentially undo or recover any unintentional modifications.
### 55. Role of the git annotate command?

In git, it is used to track each line of the file based on the commit information.

### 56. What is a git Directory?

It is the storage place of the metadata and object database of the project.

### 57. How can a conflict be settled in Git?

Edit the files to resolve any incompatible changes first, then use "git add" to add the corrected files and "git commit" to save the repaired merge.

### 58. What is the standard method for branching in GIT?

In GIT, the best way to create a branch is to have one'main' branch and then another branch for implementing the changes that we want to make.

### 59. How do you set up a Git repository?

If you want to add an empty repository to a directory in Git, use the git init command.

### 60. What is the proper syntax for appending a message to a commit?

Git commit -m "x files created" is the syntax.

### 61. Use of git instaweb?

It is used to launch a web browser and a webserver with an interface into a local repository automatically.

### 62. Describe git is-tree?

It represents a tree object with each item's mode and name included.

### 63. What exactly is git cherry-pick?

A command typically used to move specific commits from one branch of a repository to another.

### 64. State the difference between “git remote” and “got clone”?

“Git remote” allows you to create an entry in the git configuration which specify a URL.

“Git clone” lets you create a new git repository by letting you copy it from the  current URL.

### 65. Difference between “pull request” and “branch”?

“Pull request” is done when you feel like changing the developer’s change to another person's code branch. And “Branch” is just a separate version of code. 

### 66. How might you recover a branch that has previously pushed changes in the main repository yet has been coincidentally erased from each team member's local machines?

We can easily recover this by seeing the latest commit of the branch in the reflog and then going through the new branch.

### 67. What is a detached head?

Detach head refers to that the currently checked repository is not in the local branch.

### 68. What command helps us to know the branches merged into master and which are not?

git branch  - -merged lets us get the lost of the branches which are currently merged into the current branch  

git branch - - no- merged shows the branches which are not merged

### 69. Is LDAP Authentication Supported?

GitLab API only supports LDAP authentication since version 6.0 and higher.
