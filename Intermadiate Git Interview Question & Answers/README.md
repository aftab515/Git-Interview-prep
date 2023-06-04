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
