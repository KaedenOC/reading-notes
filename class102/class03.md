# Git Introduction 🖥️

## Why Do We Use Git?

Git is a DVCS (Distributed Version Control) that stores data in a file system made up of snapshots.

## Version Control

> Version Control is a system that allows you to revisit various versions of a file or set of files by recording changes. Through version control, one can revert a file or project to a previous version, track modifications and modifying individuals, and compare changes.

## Cloning In Git

Create a copy of an existing Git repository from a particular server by using the clone command with a repository's URL.

Ex: $ git clone URL

## Tracking and Staging

Single File

Track one file only by using the following format:

**git add filename**

All Files

Track all files in a repository by using the following command:

**git add (asterisk)**
> Note: After using these commands the files are tracked and staged for committing.

## Commit

After staging one or multiple files, you should commit the changes and record what you did within the commit message:


**git commit -m “made change x,y,z”**

> Note: This step has committed changes for the file or files (you can have one commit message for multiple files, if applicable) to the HEAD.

Committing All Changes

**git commit -a**
> Note: This command commits a snapshot of all modifications to tracked files in the working directory.

## Push Changes

Push changes to a remote repository.

**git push origin**

> Note: For cloned repositories, Git will automatically give the name “origin” to the server from which you cloned and the name “master” to your local repository. However, these names can be changed by the user.