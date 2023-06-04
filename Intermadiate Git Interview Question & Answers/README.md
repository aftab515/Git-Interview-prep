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
