---
title: "1st Spring Meeting"
date: 2024-01-18T12:03:49-05:00
draft: false
summary: "club meeting, Git, GitHub"
tags: ["meeting", "presentation", "GitHub"]
---

***

# Overview
- Attendance
- Git/GitHub Presentation
	- What is Git/GitHub?
	- Using Git
	- Using GitHub
	- Actually Using GitHub
	- Groupwork
	- GitIgnore
- Next Week

***

## Attendance
- Abu Shettima
- Christian Messmer
- Jonathan Buckel
- Lavender Wilson
- Matthew Williams
- Paul Shriner
- Seth Morgan
- Zach Teixido


## GitHub Presentation
### Git/GitHub
At its core, Git is version control software. To install: 
- go to [the download link](https://git-scm.com) and follow the instructions

Git works by tracking changes that are made to any source files. It then logs the changes, and keeps them stored. It essetially gives you a code history, allowing you to revert your codebase to previous versions. Proper version control makes it much easier to debug. 

GitHub is an online platform that integrates with Git in order to keep files and file histories online, allowing a higher degree of collaboration. To use it, you must create an account. Putting projects and other code on your github can be a useful tool for getting a job. 

### Using Git (via Terminal)
To create a git repository, you can run ``git init`` in any directory. A directory named ``.git`` (hidden by default) will be created; do not touch this folder. It is the root of your repository. 

You can add, remove, or change any files in the root folder. Once you're satisfied with your changes, you must add them to be tracked via the command ``git add [your files]``, or, if you want to add everything, ``git add .``. 

After adding any untracked files, you can commit them to a branch via ``git commit``. 


### Using GitHub
Most of the time, you'll be essentially copying an existing repository from online. To do this, you can fork (essentially make an online copy of a repo that you own) a repo and then clone (make a local copy) of your forked repo. For cloning, you can also do it with git in the command line with ``git clone [link-to-your-fork]``. 

After doing anything on your local repo (via ``git add``, ``git commit``, ``git restore``, etc.), you can push your changes to your local changes (only committed work) onto the remote repo (the online copy) via ``git push``. 

If your local repo is behind your remote one, you can sync your local one up to date with ``git pull``. 

### Actually Using GitHub
Chances are very high that you will rarely actually use the command line to do all your version; the vast majority of IDEs have integrated Git capabilites, and you'll use it through those (it's much easier). All the concepts are still the same (with adding, committing, pushing, pulling, etc.), but most of them will use a more visual representation (and they look nicer). 

### Groupwork: Forks, Pull Requests, and Merge Conflicts
A __fork__ is a personal copy of any repository. The fork is where all your local changes will be saved when you push changes from your local repo. It is very bad practice to upload your changes straight to the master branch; always push to your fork first, and then merge them later, once you've confirmed everything is as intended. 

A __pull request__ is a request by you to merge the changes in your fork into the master repository. In this process, your code will be peer-reviewed, and it will be either accepted or denied. After a pull request is accepted, it is final, and everything will then update to include the changes in the pull request. 

Usually, GitHub is really smart with how it handles merging. Unless you have two different files with the same file, everything will put itself together automatically. Sometimes, you'll encounter a __merge conflict__, which you will have to solve manually. The easiest way to avoid them is to work on different files than everyone else. 

### GitIgnore
Inside the root of your project, you can create a file called ``.gitignore``. Inside this file, you can specify anything you want git to ignore when tracking items. This is a very useful tool for excluding unnecessary files or folders.

```
# An example of a .gitignore file. 
# <- (comments are made using an octothorp.)

# A directory to ignore.
.\folder-name\

# A specific file to ignore.
FILENAME.txt

# A specific file type to ignore. 
*.txt
```

Generally, your dependencies take up a lot of space that could easily replace with a list of the names of the dependencies. These should be specified in your .gitignore files, but is generally handled by your package manager. 

## Next Week
Next Thursday is the Club & Org fair; We will still have a meeting, but Christian and Lavender will be at the club fair stand. The meeting will be a more relaxed meeting with a LeetCode probem or two. 
