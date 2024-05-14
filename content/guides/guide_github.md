+++
title = 'How to set up Git/GitHub'
date = 2024-05-09T22:11:03-04:00
draft = false
summary = 'Guide for using version control through Git/GitHub'
tags = ['guide', 'git']
+++

***

# Overview

- Introduction
- Creating a GitHub Account
- Setting up Git on your Computer
- Creating a Repository
- Initializing your Repository
- Using your Repository
- Conclusion

***

## Introduction

When writing code, it is important to use version control. Here are just some of the benefits of using version control:
* Comparing changes made to the codebase
* Reverting to older versions
* Learning applicable skills in the software development industry (you **NEED** to know this!)
* No more sending zip files across Discord for group projects!

To clarify: *Git* is an example of version control and *GitHub* is a platform for managing projects using Git. There are alternatives out there, but the concepts covered in this guide will apply across the board.

The following guide will cover how to get started with version control using Git/GitHub.

## Creating a GitHub Account

You can create a GitHub Account [here](https://github.com/signup). The steps are similar to any other website. Be sure to choose an appropriate username; employers may look at your GitHub!

If you are a current student, we **HIGHLY** recommend signing up for the GitHub Student Developer Pack [here](https://education.github.com/pack) to get free stuff! Who doesn't like free stuff?

## Setting up Git on your Computer

Download Git from [here](https://git-scm.com/).

Once installed, you will need to configure your username and email. This can be done with the following commands in the terminal (replace what's in the quotes with your GitHub information):

```
git config --global user.name "username"
git config --global user.email "email"
```

If you have any development environments like VS Code, be sure to sign into GitHub on them!

## Creating a Repository

On the GitHub website, go to your profile page, then the "Repositories" tab. Click on the "New" button. You should now be at the page "Create a new repository".

There are two tasks you **need** to do:
1. Enter in a repository name. It should be relevant to what you'll be using the repository for.
2. Set the visibility for your repo to Public or Private. If this is a school project, choose Private!

The other options are optional, these can be done later. You should however consider if you'll need a license (and what kind). That will be covered in an upcoming guide.

## Initializing your Repository

We will be using VS Code for this guide, but the steps are applicable to other IDEs or the command line.

The first step is to clone your new repo locally on your computer:
* In a new VS Code window, click on "Source Control" on the sidebar. 
* Click on "Clone Repository", then "Clone from GitHub". You may need to sign into GitHub. 
* Afterwards, it should show a list of your repos, choose the one you just created on the GitHub website.

Open a terminal window inside of VS Code, and follow the instructions under the section "…or create a new repository on the command line" on the GitHub website. You may add additional files to your repo folder, and you may skip the first line which creates a README.md.

Your repo is all set up!

## Using your Repository

At this point, you could do mostly everything through the VS Code GUI. Simply make changes to your files, then commit and push them through the "Source Control" panel. They will be tracked through GitHub.

But before doing so, always pull any changes from the remote branch first in order to avoid a merge conflict (and sync your repo on GitHub if you're using a fork). **Pull then push!**

Note that in a group setting, someone else might've created the main repository. In that case, you would "fork" their repository, which creates a clone on your GitHub for you to work with.

## Conclusion

This guide provides the simple steps to get started with version control using Git/GitHub if you have no experience. There are other aspects not covered by this guide that you may want to learn, such as using a ".gitignore" file, doing pull requests, and handling merge conflicts. More guides are to come that delve deeper into these topics.

For specific issues, consider checking out the [GitHub Documentation](https://docs.github.com/en/get-started/start-your-journey/about-github-and-git).

Check out our previous GitHub meetings:
* [3rd Fall 2023 Meeting](/posts/2023-09-07-3rd-fall-meeting-github-presentation/)
* [1st Spring 2024 Meeting](/posts/2024-01-18-first-spring-meeting/)

This guide was written by PennWest Software Development Club. If you have any questions, feel free to ask in our Discord or at one of our meetings. And be sure to share this guide around!
