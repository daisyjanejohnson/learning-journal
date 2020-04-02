### Git Notes

## To understand git you must first understand Version Control

- **Version Control** is a system that allows you to revisit various versions of a file or set of files by recording changes. With VC you can revert a file or project to a previous version, teack modifications and modifying individuals, and compare changes. By using a **Version Control System (VCS)**, mistakes with files can be easily fixed.
- **Local Version Control** entails one database on your hard disk that stores changes to files.
- **Centralized Version Control System (CVCS)** entails a single server storing all changes and file versions which can be accessed by carious clients. This eliminates the need to involve all local databases and allows programmers to have more knowledge of other people's activities with certain files and gives administrators the ability to divy up revision priveledges. 
- **Distributed Version Control Systems (DVCS)** allows clients to create mirrored repositories, these data backups can be placed on the server to replace any lost information.

## What is Git?

* Git is a DVCS that stores data in a file system made of snapshots. Each time you save a changed version of your project, Git creates a snapshot of the file and stores a reference to it.
* Every single change applied to any file or directory is tracked by Git. Git always detects file corruption or loss of information in transit.
* Git minimizes the possibility of irreversible damage to files, like accidentally lost data.
* Files in Git reside in three main states:
  * **Committed**- Data is securely stored in a local database.
  * **Modified**- File has been changed but not committed to the database.
  * **Staged**- Flagged a file's changed version to be committed in the next snapshot.
  
To use Git, your computer must have it available and it must be the latest version. [Thislink has instructions on how to download Git onto your computer and also how to set up a Git Repository](https://www.udemy.com/blog/git-tutorial-a-comprehensive-guide/)

You can access the manual on Git to get more info on a particular command by using one of three different codes:
```
git help command
git command --help
man git-command
```
# Workflow

***Local Repository Structure***

**The local Git repository has three components:**
  1. Working Directory: The actual files reside here.
  1. Index: The area used for staging.
  1. Head: Points to the most recent commit.
  
***Saving Changes***

**All files in a checked out (working) copy of a project file are either in a tracked or untracked state**
- ***Tracked***- Tracked files can be modified, unmodified, or staged. Were part of the most recent file snapshot.
- ***Untracked***- Untracked files were not in the last snapshot and do not currently reside in the staging area
- _After cloning a repo, files are tracked and unmodified because they have been checked out but not edited_

***Life Cycle of the Status***

1. After editing a file, Git flags it as modifies becaus changes made after the previous commit.
1. You stage the modified file.
1. Then, you commit staged changes.

- To determine the state of files, use the `git status` command.

***Tracking and Staging a New File***

* __Single File__- Track one file by using the following format: `git add filename`
* __All Files__- Track all files ina repository by using this command: `$ git add *`

***Commiting a File***

After staging one or multiple files, commit the changes and record what was done in the commit message: `$ git commit -m "made change x,y,z"`

***Committing All Changes***

* To commit a snapshot of all modifications to tracked files in the working directory use the command: `$ git commit -a` 

***Pushing Changes***

After commiting changes, push changes to a remote repository with command: `$ git push origin master`

