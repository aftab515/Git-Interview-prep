# Popular Git Interview Questions & Answers

## Written by <https://github.com/aftab515>

### 70. What's the simple definition of Git?

Git is a free and open-source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.

### 71. Is the C++ language used in Git?

Yes, but C programming language is a widely used language in Git.

### 72. How does Git work?

Git works by tracking changes to files in a project and allowing developers to easily revert to previous versions if necessary. Git also makes it easy to collaborate on projects, as it allows multiple developers to work on the same codebase simultaneously.

### 73. What are some of the most popular Git commands?

Some of the most popular Git commands are,

- "git init" (which initializes a Git repository)
- "git add" (which adds files to a Git repository)
- And "git commit" (which saves changes to a Git repository).

### 74. List out the functions provided by Git repository hosting service?

There are many functions that a Git repository hosting service can provide. Some of the most common and useful functions include:

- Providing a web interface for users to interact with the repositories.
- Allowing users to clone repositories.
- Allowing users to view and download statistics about the repositories.
- Providing a way for users to push changes to the repositories.
- Keeping track of changes made to the repositories.

### 75. What is the difference between Git and other revision control systems?

- Git is a distributed revision control system, which means that it can be used without a central server. This allows for a great deal of flexibility in how projects are managed.
- On the other side, revision control systems are often centralized, which can limit the flexibility of how projects are managed.

### 76. How does Git work?

Git works by tracking changes to files in a repository. When a file is changed, Git calculates a unique identifier for the change, called a "commit hash". The commit hash allows Git to identify the change and track it over time.

### 77. How do I install Git?

Installing Git is simple. Just download the latest version from the Git website (<https://git-scm.com/>).  

### 78. How do I use Git?

To use Git, a developer first creates a local repository on their computer.
This repository contains all the files for a project and the history of all the changes made to those files.

Or just follow the instructions in the Git documentation (<https://git-scm.com/doc>).

### 79. What are some of the drawbacks of Git?

- One of the main drawbacks is that it can be difficult to learn and use, especially for those who are not familiar with version control systems.
- And Git is not always reliable and can sometimes be slow.

### 80. What are some of the most important commands in Git?

Some of the most important Git commands are "commit", "push", and "pull".

- The "commit" command is used to save changes to the local repository.
- And the "push" command is used to send changes to the remote repository.
- Then the "pull" command is used to retrieve changes from the remote repository.

### 81. What are some of the most important features of Git?

Some of the most important features of Git are its distributed nature, its ability to track changes, and its support for branches.

- The distributed nature of Git allows developers to work independently and offline.
- The ability to track changes helps developers to keep track of their work and revert to previous versions if necessary.
- The support for branches allows developers to experiment with new features without affecting the main codebase.

### 82. What is a branch in Git?

A branch is a way to isolate development work on a particular aspect of a project. When a branch is created, it diverges from the primary branch. It allows developers to work on a new feature or bug fix without affecting the main codebase.

### 83. What is a commit in Git?

A commit is a way to save changes to a branch. When a commit is made, a snapshot of the current state of the branch is created. This snapshot can be used to revert the branch to that state if necessary.

### 84. What is conflict in Git?

Conflict in Git occurs when two or more developers have made changes to the same part of a file, and those changes can't be automatically merged. When this happens, Git will mark the file as conflicted and leave it up to the developers to resolve the conflict.

Resolving a conflict can be done by manually editing the file to choose which changes should be kept, or by using a tool like Git's merge command to automatically merge the changes.

### 85. What does the git status command do?

The git status command is used to obtain the current state of a Git repository. This command can be used to determine whether the repository is clean or dirty, and to see which files have been modified. The git status command will also show which branch is currently checked out and whether there are any uncommitted changes.

### 86. Why is it considered to be easy to work on Git?

There are many reasons that Git is considered an easy tool to work with.

- It has a straightforward learning curve. Even those new to programming can easily learn how to use Git with just a few hours of practice.
- Git is highly flexible and can be easily customized to fit the needs of any project.
- And, Git is very stable and reliable, so users can trust that their work will be safe and sound.

### 87. What do you know about Git Stash?

Git stash is a powerful tool that allows you to save your changes and revert your working directory to a previous state. This is especially useful when switching branches or reverting to a previous commit.

And Git Stash takes a snapshot of your changes and stores them away for later use.

### 88. What differentiates between the commands git remote and git clone?

The main difference between the git remote and git clone commands is that the git remote adds a remote repository as a shortcut to your current repository, while the git clone creates an entirely new copy of a remote repository.

### 89. Tell me the difference between git pull and git fetch?

Both of these commands will fetch any new commits from the remote repository, but they differ in how they handle these commits.

Git pull will merge the remote commits into the current branch, while git fetch will simply retrieve the commits and store them in the local repository. This means that if you have any uncommitted changes, git pull may result in merge conflicts, while git fetch will not.

### 90. Is Git and GitHub the same thing?

No, Git and GitHub are two different things.

- Git is a version control system that lets you track changes to your code.
- GitHub is a hosting service for Git repositories. You can use GitHub to store your code remotely, or you can use it to collaborate with other developers on a project.

### 91. What about Git reflog?

Git reflog is a history of all the changes made to a git repository. It is a valuable tool for debugging and troubleshooting purposes.

And Git reflog can be used to view the history of a repository, see who made what changes, and when those changes were made.

### 92. What is a detached head?

A detached HEAD is a state where the HEAD pointer is not pointing to the current commit. This can happen if you check out a commit that is not the most recent, or if you reset your head to a previous commit.

### 93. How to avoid a detached head?

There are a few different ways to avoid a detached HEAD.

- The first is to simply commit your changes before switching branches. This will ensure that your changes are saved to a specific branch, and you won't have to worry about them being lost when you switch branches.
- Another way to avoid detached HEAD is to use the "git checkout" command with the "-b" option.

### 94. How will you resolve conflict in Git?

To resolve a conflict in Git, you will need to first identify the source of the conflict. Once you have identified the source of the conflict, you can use the "git pull" command. This will pull the latest changes from the remote repository and merge them with your local copy.

If the "git pull" command doesn't resolve the conflict, you can try the "git merge" command. This will merge the two versions of the code manually. You will need to resolve the conflicts manually and then commit the merged code.

### 95. What is Subgit and where do you use Subgit?

Subgit is a tool for managing Git repositories with Subversion history. It allows you to keep your existing subversion history while moving to Git, and it also provides a way to keep your Git history synchronized with subversion.

There are many reasons that you might want to use Subgit;

- For example: if you have a large subversion repository with a lot of history, moving to Git can be a huge undertaking; that's where Subgit can help transition smoother.
- And if you work in an environment where subversion is the primary version control system, using Subgit can help you keep your Git history in sync with the rest of the team.
