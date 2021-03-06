# What are Git and GitHub? {#Git2}



Trying to find instructions on how to use git and GitHub online is notoriously difficult for beginners. You'll often come across instructions like this:

> Doing X is easy. All you have to do is open up a terminal and type
>
> `git -s -x -what -thehell -doesthisallevenmean`

Thankfully, using Git and GitHub doesn't have to be this hard! You don't even have to use the command line at all to benefit from these tools.

To get started, it is important to know what Git and GitHub are and how they differ.

## Git {#Git2.1}

*Git* is software that (usually) runs on your computer. It is used to track all changes within a particular folder. Any change within that folder --- a deleted file, a new line in a file, or a single changed letter in a single file --- is tracked. It's as if Microsoft word's "Track Changes" function donned a cape, started solving crime, and kept meticulous notes all the while.

A folder on your computer that is tracked by Git is called a `repository` or `repo` for short. The main difference between a Git repo and a regular folder on your computer is that a Git repo has a folder within it named `.git`. It's within this `.git` folder that all the changes in the main folder are tracked. Other than that, a Git repo is just a folder on your computer like any other, but with new and wonderful powers.

## GitHub {#Git2.2}

*GitHub* is an internet service that provides online cloud hosting for Git repos, as well as useful tools for sharing and collaboration. You don't have to have a GitHub account to use Git, and you don't have to have Git installed on your computer to use GitHub. But if you want a cloud backup, want to sync your work to multiple computers, or especially if you want to collaborate or share your work with others (or use/contribute to their work!), you'll want to use both Git and GitHub.

> **Git** tracks all changes within a particular folder (aka git repo) on your computer

> **GitHub** offers a way to backup or sync your Git repos, or to collaborate with others

<img src="images/Git0.PNG" width="700px" style="display: block; margin: auto;" />

Image credit: devmountain.com

If you're a fancy pants programmer you may want to use Git from the command line (e.g., terminal or bash depending on your situation) so you can look cool, and admittedly have more fine-grained control over the process. But if you're like the rest of us, and if you're reading this document right now, you may want a more user- and beginner-friendly option.

## Git the language? {#Git2.3}

Were you the kid that was tormented by your siblings speaking Pig Latin (also known as "Igpay Atinlay") and no matter how hard you tried, you couldn't figure it out? Learning to use Git and GitHub can feel like learning a new language. But we promise it is easier than Pig Latin.

When working with Git and GitHub, you are going to see the words `repo`, `origin`, `commit`, `push`, `pull`, `clone`, `fork`, and `branch`, among others. We will start with some basic definitions here, and in later chapters will elaborate on terms as necessary.

**repo(sitory)** - a folder whose contents are is tracked by Git. A repo can exist locally (on your computer) as a remote repository (on GitHub), or both.

**origin** - the primary Git repo, against which other copies are compared. In our examples, we will create the origin repo in GitHub

**push** - send changes from your local Git repo to the remote repository (e.g. GitHub)

**pull** - get changes from the cloud and updates your local Git repo

> Note: this is different from a `pull request` which is when you want someone else to incorporate your changes into their GitHub repo. More on this later.

**commit** - create a named version of a set of one or more changes to a local Git repo. Like a bookmark of the current changes made. Often will be pushed to GitHub, but can be local only. To add to the confusion, `commit` in Git language can be a verb and a noun! In other words, when you commit your changes, you create a commit.

**clone** - create a copy of a Git repo maintaining a direct link to the original repository. In our examples, the repos will first be created on GitHub (i.e., origin) and then *cloned* to your local Git repo on your computer.

> Note: if you clone a repo from someone else GitHub account, you cannot contribute to their repo unless they have given you access, but if you do you are contributing directly to the repository.

**fork** - create a copy of a repo which maintains a loose connection between your local repo and the origin repo. Think of a fork as a bridge between the original repo and the local copy where changes can be made. After making and testing changes, you can contribute back to the original repo using a `pull request` which must be approved by the repository owner.

**branch** - new/separate versions of the repo. It is a way to modify your scripts, while not changing your original code. If you're happy with your changes you can eventually merge them into your original code. It is a feature in most version control systems.

> Note: the primary or default branch in Git is the `master branch` (sometimes referred to as `main` branch). Think of the master branch as the trunk of the tree. Every repo contains at minimum this one branch, which is created when the repo is initialized. If you want to test new changes, you would create another branch which could then be merged later. More on this later!

## Git to GitHub GUIs {#Git2.4}

There are multiple graphical interfaces for using Git and GitHub. This document will provide instructions for two methods: [GitHub Desktop](#Desk3) and [RStudio](#RStud4).

Q: Which option is for you??

A: It depends. GitHub Desktop and RStudio offer different advantages. Which is best for you will largely depend on how you plan to use and interact with GitHub.

-   If you are not actively developing R code, and/or just need to get existing files into GitHub, GitHub Desktop is the easiest method, with the least amount of configuration.

-   If you are actively writing analytical scripts in R, then using RStudio is recommend because there will be some additional instructions for using `R Projects` to organize your workflow and annotate your code.

You can use multiple Git GUIs at the same time without any issues so feel free to set up and get familiar with both.

## Getting Started {#Git2.5}

Regardless of the GUI you choose to use, there are a few steps you need to take to get started.

First, get the software and account that you need:

1.  Download and install `git` on your computer from here: <https://git-scm.com/downloads>

<img src="images/Git1.PNG" width="700px" style="display: block; margin: auto;" />

> Note: Most linux users will already have `git` installed, or should use their system's repositories to install `git`

2.  Sign up for a GitHub account here: <https://github.com/join>

<img src="images/Git2.PNG" width="700px" style="display: block; margin: auto;" />

Now you are ready to become a Git master! [Chapter 3](#Desk3) will get you started with GitHub Desktop and [Chapter 4](#RStud4) will get you started with RStudio.

Some elements of these Chapter are repetitive so that users can choose one or the other. If you choose to go with both, then skim over the repetitive parts.

Choose your own adventure!
