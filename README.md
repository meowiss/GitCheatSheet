# GIT CHEATSHEET

## 🌹 What is Git ? 

Git is a Version Control system (VCS). Version Control System is a system that records the changes we make on a document, such as a project or a document, step by step and allows us to store and manage it in a repository on the internet if you want. Git, SVN, BitKeeper, and Mercurial are examples of version control systems. First of all, let's underline that the expression version is the state of the files at any time they are recorded. Version control (also revision control or source control) is when changes (editing, deleting, adding, renaming) to one or more files (can be text files, images, text and media files, executable applications, and more). It is a system that makes it possible to record and track (change, copy, etc.) and  return to specific action points versions/versions) when necessary.

![](https://i.imgur.com/ntwao7Y.png)

## 🎨 Most Frequent Git Commands

here are frequently used git commands I'd like to share it :) 🌺
* `Git init`: Initializes a new Git repository.
* `Git config`: Sets the author name and e-mail address with the values given.
* `Git commit`: defines the basic workflow for all developers. It takes the staged snapshot and commits it to the project history also can be conbined with `git add` as it like `git add-commit -m 'commit message'`
* `Git status`: It displays the state of the working directory and the staged snapshot. The changes we have made in the files can be seen by using this command.
* `Git log`: Shows the project directory. This command can be used as `git log --oneline` so that we can see the commits more practical way.
* `Git branch`: General-purpose branch administration tool, but I have used it to create isolated development environments within a single repository.
*  `Git checkout`: Checks commits and revisions. In addition, navigates/travels around existing branches.
*  `Git merge`: It merges a branch with the “master” or “main” branch.
*  `Git remote`: A mutual repository that all of my team used to make their changes. It can be used by passing the URL of the shared repository.
*  `Git push`: Uploads the working or local branch to another repository.
*  `Git pull`: Downloads a branch from a remote repository and quickly merges it into the current branch.
*  `Git rm`: Removes a file from the Git workspace.
*  `Git diff`: Compares the differences between two commits.
*  `Git clone`: Git clone allows us to copy a repository to our local-machine. 


---

# 🌟 A List of Git Commands


## 🌱 Git Setup

📌 **Create a new Git repository** from an existing directory:
```
git init [directory]
```
📌 **Clone a repository** (local or remote via HTTP/SSH):
```
git clone [repo / URL]
```
📌 **Clone a repository** into a specified folder on your local machine:
```
git clone [repo / URL] [folder]
```

## ✏️ Git Configuration

📌 Attach an **author name** to all commits that will appear in the version history:
```
git config --global user.name "[your_name]"
```
📌 Attach an **email address** to all commits by the current user:
```
git config --global user.email "[email_address]"
```
📌 Apply Git’s automatic command line coloring which helps you keep track and revise repository changes:
```
git config --global color.ui auto
```
📌 Create a shortcut (alias) for a Git command:
```
git config --global alias.[alias_name] [git_command]
```
> **Note**: Git requires you to type out the entire command to perform actions. Setting shortcuts for commonly used commands can speed up and simplify development. For example, you can use the alias **st** for the status command by typing the command: git config --global alias.st status``

📌 Set a **default text editor**:
```
git config --system core.editor [text_editor]
```
📌 Open Git’s **global configuration file**:
```
git config --global --edit
```
## 📒 Manage Files

📌 Show the state of the **current directory** (list staged, unstaged, and untracked files):
```
git status
```

📌 List the **commit history** of the current branch:
```
git log
```

📌 List **all commits** from all branches:
```
git log --all
```
📌 **Compare two branches** by showing which commits from the first branch are missing from the second branch:
```
git log [branch1]..[branch2]
```
📌 Examine the **difference** between the **working directory and the index**:
```
git diff
```
📌 Explore the difference between the **last commit and the index**:
```
get diff --cached
```
📌 See the difference between the **last commit and the working directory**:
```
get diff HEAD
```
📌 Display the **content and metadata** of an object (blob, tree, tag or commit):
```
git show [object]
```

## 🪴 Git Branches

📌 List **all branches** in the repository:
```
git branch
```
📌 List **all remote branches**:
```
git branch -aa
```
📌 Create a new branch under a specified name:
```
git branch [branch]
```
📌 **Switch** to a branch under a specified name (if it doesn’t exist, a new one will be created):
```
git checkout [branch]
```
📌 **Delete Local Branch**:
```
git branch -d [branch]
```
📌 **Rename** you are currently working in:
```
git branch -m [new_branch_name]
```
📌 **Merge** the specified branch **with the current branch**:
```
git merge [branch]
```

## 📑 Make Changes

📌 Stage changes for the next commit:
```
git add [file/directory]
```
📌 Stage everything in the directory for an initial commit:
```
git add .
```
📌 Commit staged snapshots in the version history with a descriptive message included in the command:
```
git commit -m "[descriptive_message]"
```
## ✂️ Undo Changes

📌 Undo changes in a file or directory and create a new commit with the command:
```
git revert [file/directory]
```
📌 unstage without overwriting changes:
```
git reset [file]
```
📌 Undo any changes introduced after the specified commit:
```
git reset [commit]
```
📌 Show untracked files which will be removed:
```
git clean -n
```
📌 Remove untracked files:
```
git clean -f
```

📌 Replace the last commit with a combination of the staged changes and the last commit combined:
```
git commit --amend
```
📌 Rebase the current branch with the specified base (it can be a branch name, tag, reference to a HEAD, or a commit ID):
```
git rebase [base]
```
📌 List changes made to the HEAD of the local repository:
```
git reflog 
```
## 🏝️ Remote Repositories
📌 Create a new connection to a remote repository (give it a name to serve as a shortcut to the URL):
```
git remote add [name] [URL]
```
📌 Fetch a branch from a remote repository:
```
git fetch [remote_repo] [branch]
```
📌 Fetch a repository and merge it with the local copy:
```
git pull [remote_repo]
```
📌 Push a branch to a remote repository with all its commits and objects:
```
git push [remote_repo] [branch]
```

## 🎊 Summary
In this repo, I tried to summarize and mention about git commands and how to use them. I hope you really enjoyed from this small-writeup :) , thank you for reading ✨💛

btw at last but not least here are my resources :D

## ✉️ Resources

https://git-scm.com/
