+++
title = '3rd Fall Meeting - Git + GitHub Intro'
date = 2023-09-07T11:00:00-12:00
draft = false
summary = 'logo status, faculty advisor, club meeting'
tags = ['technologies', 'git', 'presentation']
+++

# Attendance

- Abu Shettima
- Zachary Teixido
- Matthew Williams
- Jeremiah Neff
- Christian Messmer
- Brandon Mastin
- David
- Gage
  
# Summary

- We encouraged all club members to create a GitHub account, join the [club organization](https://github.com/pwsdc), and create a pull request.
- We continued our discussion with game or project ideas for the club.
- The Career Center mentioned that Erie Insurance was possibly interested in talking about internship opportunities. However, there has been no confirmation from Erie Insurance at this time.

# Git Discussion

## Background

- **Git** is a local binary that runs on your computer.
- **Git** is a software solution for **version control**.
- The purpose of Git is to save the current state of your entire directory.
- **GitHub** and **BitBucket** are examples of cloud hosting services.
- These services make it very easy to share your code.
- The concept is similar to a tree structure. People edit their "nodes", and merge the updates together, into the master branch.

## Installing Git on Windows

- Download Git for Windows [here](https://git-scm.com/download/win)
- In the installer, most default options will suffice. (**Exception: Vim is the default text editor. We do not recommend this option. Select VS Code from the drop-down menu.**)
- After navigating the installer, open your command-line, and type `git`. This will ensure it has installed properly.

## Git Command-Line

These commands will be entered via command-line. (Hint: use `dir` and `cd C:\go\to\this\directory` commands to navigate to your desired folder)

`git init`
This will setup your current directory with git. **Use this command FIRST to setup a project in a local, newly created folder!**

`git clone https://github.com/link/to/a/repo`
This will download a project from a cloud hosting service, like GitHub.

`git config --global user.name "My Name"` 
Set your global username. **Required for the Git GUI in VS Code**.

`git config --global user.email "Email@Email.com"`
Set your global email. **Required for the Git GUI in VS Code**.

`git status`
Retrieves information about your project. (Such as the current branch you are using)

`git add *`
Prepares all untracked (newly created) files to be committed. **Typically, you would do this before a commit.**

`git commit -m "Here is a basic summary of my newest contributions."`
Commits all tracked files, along with a message. Ideally, the message should provide relevant information.

`git remote add origin https://github.com/pwsdc/example-repo`
Upload a local repository to a new GitHub repository.

`git push`
Upload your local changes to GitHub. **Ensure your local repository is connected to a GitHub repository**, using the command provided above.

## Git Integration with VS Code

- When you open VS code, focus on the left-most panel. There should be an icon for "**source control**" (The icon resembles a tree with nodes).
- The GUI will provide ways to initialize Git, add untracked files, commit changes, and push commits.
- The GUI is much more user friendly, but the console is much more powerful.

# Members Made Pull Requests 

- Everyone was encouraged to pull request to the [Resources repository](https://github.com/pwsdc/resources) in the [club organization](https://github.com/pwsdc/).
- We received contributions from `mwilliams52000`, `BrandonM03`, and `DTBdude`, where Karl merged their changes into the master branch.

# Game Ideas

- Christian suggested a fighting game against the three mascots from the three campuses.
- He suggested that we would need a game engine.
- There were suggestions to use M.U.G.E.N. We looked into GitHub to find a pre-build project to use as a base.

# Votes

No votes were held this meeting.

# Agenda for Next Meeting (Sep 14 2023)

- Karl and Paul will not be present during the meeting. They will be attending the club fair, in hopes to promote the club.
- Christian plans to prepare a PowerPoint presentation on VS Code, and continue the discussion for our game idea.
