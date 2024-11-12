+++
title = '11th Fall 2024 Meeting'
date = 2024-11-12T17:40:05-05:00
draft = true
summary = 'intro to version control'
tags = ['git', 'version control', 'elections']
+++
***
# Overview
- Attendance
- Officer nominations
- Git Discussion
- Next Week
***

# Attendance
Officers:

- Abu Shettima
- Lavender Wilson
- Matthew Williams
- Paul Shriner

Members:

- Chibuikem Asuzu
- DaJuan Bowie
- Jonathan Buckel
- Kevin Kauffman
- Maddox Miller
- Michael Paterno

# Officer nominations
Officer nominations are now open! All positions (President, Vice President, Treasurer, and Secretary) are open. Someone can nominate themself or someone else using the Discord channel that will be created shortly after this meeting. Descriptions of officer positions can be found within our [club's constitution](https://engage.pennwest.edu/organization/caprogra/documents/view/2232118). 
Those nominated will give brief remarks at next week's meeting and then we will vote for the candidates through Engage.

# Git Discussion
## What is Git?
Git is a way to facilitate version control within a group setting. It is an industry standard, most companies will use some form of version control.

Git provides:
- History of directory
- Branches 

## Untracked Files
These are files that exist in your working directory but are not being tracked by Git. They have not been added to the staging area and will not be included in commits unless explicitly added. You can use a ```.gitignore``` file to specify patterns for files that Git should ignore, preventing them from being tracked.

## Tracked Files
Tracked files are files that Git is monitoring. They can be in one of the following stages: modified, staged, and committed.

### Modified
The file has been changed in the working directory since the last commit, but those changes have not yet been staged for the next commit.

### Staged
The file has been modified and the changes have been added to the staging area (using ```git add```). It is ready to be included in the next commit.

### Committed
The changes in the staged files have been saved to the repository's history. This means that the changes are now part of the project's version history and can be shared with others.

## VS Code Integration
Git version control can be utilized in VS Code. Changes in the file can be tracked, such as removals or additions, and then staged for commits. Lavendar showcased several features in VS Code, such as handling commits and branching along with merging commits.
Someone with industry experience mentioned that it is unlikely that commits will directly be merged into 'main'.

## Merge Conflicts
Merge conflicts occur when two different commits work on the same piece of code. As a result, Git does not know how to handle it, i.e which piece of code should be used moving forward. It is possible to handle merge conflicts in a merge editor, in which the reviewer can fix the conflict by writing a unified solution. Lavendar showcased an example of creating a merge conflict and resolving one in VS Code using the command line and the merge editor.

## Installing Git
Git is integrated in VS Code. To use it system wide, Windows users must install Git from [here](https://git-scm.com/downloads). Make sure Git Bash is installed during this process!

## Making a local repo
Open a folder from within a terminal and type ```git init```. Alternatively, a folder can be opened in VS Code and then initialized into a local repo on the Source Control panel.

# Next Week and Beyond
Next week, at the same date and time as usual, we will hold an election for the Spring 2025 officers. Additionally, the club is planning on holding a pizza party on **December 3rd**. Stay tuned for more info!