# Table of Contents
- [Table of Contents](#table-of-contents)
  - [Termoinologies](#termoinologies)
    - [&nbsp;&nbsp;&nbsp;&nbsp; Branch](#-branch)
    - [&nbsp;&nbsp;&nbsp;&nbsp; Checkout](#-checkout)
    - [&nbsp;&nbsp;&nbsp;&nbsp; Clone](#-clone)
    - [&nbsp;&nbsp;&nbsp;&nbsp; Commit](#-commit)
    - [&nbsp;&nbsp;&nbsp;&nbsp; Git <a href="https://www.freecodecamp.org/news/learn-the-basics-of-git-in-under-10-minutes-da548267cc91/">source</a>](#-git-source)
    - [&nbsp;&nbsp;&nbsp;&nbsp; Repository](#-repository)
    - [&nbsp;&nbsp;&nbsp;&nbsp; Staging Area <a href="https://dev.to/sublimegeek/git-staging-area-explained-like-im-five-1anh">source</a>](#-staging-area-source)
    - [&nbsp;&nbsp;&nbsp;&nbsp; Version Control](#-version-control)
  - [Setting Up the Environment](#setting-up-the-environment)
    - [&nbsp;&nbsp;&nbsp;&nbsp; 1. Install Git](#-1-install-git)
    - [&nbsp;&nbsp;&nbsp;&nbsp; 2. Setup your username and email](#-2-setup-your-username-and-email)
  - [Basic Commands](#basic-commands)
    - [&nbsp;&nbsp;&nbsp;&nbsp; git add](#-git-add)
    - [&nbsp;&nbsp;&nbsp;&nbsp; git clone](#-git-clone)
    - [&nbsp;&nbsp;&nbsp;&nbsp; git log](#-git-log)
    - [&nbsp;&nbsp;&nbsp;&nbsp; git status](#-git-status)
  - [Some UseCase Guides](#some-usecase-guides)
    - [&nbsp;&nbsp;&nbsp;&nbsp; Creating a local repository](#-creating-a-local-repository)
    - [&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1. Create a new repository on Github](#-1-create-a-new-repository-on-github)
    - [&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2. Choose a directory for your repo](#-2-choose-a-directory-for-your-repo)
    - [&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 3. Open Git Bash](#-3-open-git-bash)

<br>
<br>
<br>
<br>
<br>
<br>
<br>

## Termoinologies
### &nbsp;&nbsp;&nbsp;&nbsp; Branch
- a version of a repository
- a repository can have many branches (eg. master/main, feature, development)
- why are multiple branches needed?  
  - Multiple branches are needed to support multiple parallel developments. Refer the image below to see how branches work. <a src="https://www.freecodecamp.org/news/what-is-git-and-how-to-use-it-c341b049ae61/">source</a>
  - <img alt="branch-image1"  src="https://cdn-media-1.freecodecamp.org/images/sww3mboJ61C4kpLWlQYHnHWvrjX8p--VMui2"/>



<br>

### &nbsp;&nbsp;&nbsp;&nbsp; Checkout
- means switching between to different versions of a repository

<br>

### &nbsp;&nbsp;&nbsp;&nbsp; Clone
- copy or CLONE a repository to your machine

<br>

### &nbsp;&nbsp;&nbsp;&nbsp; Commit
- a commit is a collection of: 
  - content
  -  a message about how you got there 
  -  and the commits that came before it. <a href="https://opensource.com/article/19/2/git-terminology">source</a>

- a snapshot of the project's staged changes. <a href="https://www.atlassian.com/git/tutorials/saving-changes/git-commit#:~:text=The%20git%20commit%20command%20captures,you%20explicitly%20ask%20it%20to.">source</a>
  
- As a noun: A single point in the Git history; the entire history of a project is represented as a set of interrelated commits. The word "commit" is often used by Git in the same places other revision control systems use the words "revision" or "version". Also used as a short hand for commit object. <a href="https://stackoverflow.com/questions/43970559/what-is-exactly-meaning-of-commit-command-in-git">source</a>

- As a verb: The action of storing a new snapshot of the project’s state in the Git history, by creating a new commit representing the current state of the index and advancing HEAD to point at the new commit. <a href="https://stackoverflow.com/questions/43970559/what-is-exactly-meaning-of-commit-command-in-git">source</a>

<br>

### &nbsp;&nbsp;&nbsp;&nbsp; Git <a href="https://www.freecodecamp.org/news/learn-the-basics-of-git-in-under-10-minutes-da548267cc91/">source</a>
- Git is a version-control system for tracking changes in computer files and coordinating work on those files among multiple people. 
- Git is a Distributed Version Control System. 
- Git helps you keep track of the changes you make to your code. It is basically the history tab for your code editor(With no incognito mode ?).

<br>

### &nbsp;&nbsp;&nbsp;&nbsp; Repository 
- a collection of cource code

<br>


### &nbsp;&nbsp;&nbsp;&nbsp; Staging Area <a href="https://dev.to/sublimegeek/git-staging-area-explained-like-im-five-1anh">source</a>
- the <ins>staging area is like a box</ins> where you can put stuff into it and take stuff out of it.
  - any change you make becomes a thing that is outside of the box
  - before you want to execute <ins>git commit</ins>, you have to put things inside of that box.
- <img src ="https://cdn-images-1.medium.com/max/800/1%2AdiRLm1S5hkVoh5qeArND0Q.png" />

<br>

### &nbsp;&nbsp;&nbsp;&nbsp; Version Control
- Version control is a system that records changes to a file or set of files over time so that you can recall specific versions later. So ideally, we can place any file in the computer on version control. <a href="https://www.freecodecamp.org/news/learn-the-basics-of-git-in-under-10-minutes-da548267cc91/">source</a>

<br>
<br>
<br>
<br>
<br>
<br>
<br>

## Setting Up the Environment
### &nbsp;&nbsp;&nbsp;&nbsp; 1. Install Git
   - Go to <a href="https://git-scm.com/downloads">Git Downloads Page</a>
   - Install compatible version

<br>

### &nbsp;&nbsp;&nbsp;&nbsp; 2. Setup your username and email
   - On any directory, right click and select "Git Bash Here"
   - Input the following commands: 
      ```git
         git config --global user.name your-username-here
      ```
      - to enter your username
      ```git
         git config --global user.name your-email-here
      ```
      - to enter your email
      - to check if the configuration was properly set up: 
         ```git
            git config --list
         ```
        - then  look  for  user .name  and  user .email
        - asdfasdfasdf


<br>
<br>
<br>
<br>
<br>
<br>
<br>


## Basic Commands
### &nbsp;&nbsp;&nbsp;&nbsp; git add
   - ```
      git add .
     ```
     - add all changed/new files to staging area
   - ```
      git add file1 file2 file3
     ```
        - add specific files to staging area
      git add filename
     ```
        - add a single file to the staging area

<br>
<br>


### &nbsp;&nbsp;&nbsp;&nbsp; git clone

- ```git
   git clone https://repository.url
   ```
    - copy a repository into your chosen directory

<br>
<br>

### &nbsp;&nbsp;&nbsp;&nbsp; git commit
 - ```git
   git commit -m "commit message"
   ```
   - create a snapshot of the project for uploading via git push
   git init
   ```
   - initialize a repository

<br>
<br>

### &nbsp;&nbsp;&nbsp;&nbsp; git init
 - ```git
   git init
   ```
   - initialize a repository

<br>
<br>

### &nbsp;&nbsp;&nbsp;&nbsp; git log
 - ```git
   git log
   ```
   - print out all the commits up to the latest
   - to exit after executing the command, press q

<br>
<br>

### &nbsp;&nbsp;&nbsp;&nbsp; git push
 - ```git
   git push
   ```
   - check which files have been changed / are new

<br>
<br>

### &nbsp;&nbsp;&nbsp;&nbsp; git status
 - ```git
   git status
   ```
   - check which files have been changed / are new

<br>
<br>

### &nbsp;&nbsp;&nbsp;&nbsp; git status
 - ```git
   git status
   ```
   - check which files have been changed / are new

<br>
<br>


## Some UseCase Guides
### &nbsp;&nbsp;&nbsp;&nbsp; Creating a local repository
### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1. Create a new repository on Github
   - <img src="https://docs.github.com/assets/images/help/repository/repo-create.png">
### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2. Choose a directory for your repo
### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 3. Open Git Bash


