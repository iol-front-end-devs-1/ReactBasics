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
    - [&nbsp;&nbsp; a.) Creating a local repository](#-a-creating-a-local-repository)
    - [&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1. Create a new repository on Github](#-1-create-a-new-repository-on-github)
    - [&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2. Choose a directory for your repo](#-2-choose-a-directory-for-your-repo)
    - [&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 3. Open Git Bash](#-3-open-git-bash)
    - [&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 4. Initialize the directory as a git repository](#-4-initialize-the-directory-as-a-git-repository)
    - [&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 5. Add files, inside the directory, to the staging area.](#-5-add-files-inside-the-directory-to-the-staging-area)
    - [&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 6. Commit the files inside the staging area](#-6-commit-the-files-inside-the-staging-area)
    - [&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 7. Copy the remote repository URL.](#-7-copy-the-remote-repository-url)
    - [&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 8. In the git bash, add the remote repository URL](#-8-in-the-git-bash-add-the-remote-repository-url)
    - [&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 9. Push the changes to your reposirtory.](#-9-push-the-changes-to-your-reposirtory)
    - [&nbsp;&nbsp; b.) Getting the latest updates from the repository](#-b-getting-the-latest-updates-from-the-repository)

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


### &nbsp;&nbsp;&nbsp;&nbsp; git remote
 - ```git
   git remote add repo-name https://repository.remote.urlHere
   ```
   - sets a new remote url that you can use
 - ```
      git remote -v 
   ```
   - verifies the remote url 

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


## Some UseCase Guides

### &nbsp;&nbsp; a.) Creating a local repository

<br>

### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1. Create a new repository on Github
   - <img src="https://docs.github.com/assets/images/help/repository/repo-create.png"/>

<br>

### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2. Choose a directory for your repo

<br>

### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 3. Open Git Bash

<br>

### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 4. Initialize the directory as a git repository 
  -  ```git
         git init
      ```
      
<br>

### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 5. Add files, inside the directory, to the staging area.
   - ```git
      git add .
      #this command adds all files in the directory to the staging area.

      #to unstage a file
      git reset HEAD file-name
     ```
<br>

### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 6. Commit the files inside the staging area
   - ```git
      git commit -m "inital commit"


      #to remove a commit
      git reset --soft HEAD~1
     ```
### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 7. Copy the remote repository URL.
   - at the top of your GitHub repository's Quick setup page, click the the clipboard icon to copy the remote repository URL.
   - <image src="https://docs.github.com/assets/images/help/repository/copy-remote-repository-url-quick-setup.png">
### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 8. In the git bash, add the remote repository URL
   - ```
      git remote add origin https://repository.remote.url
      #to set the new remote URL
      git remote -v 
      #to verufy the new remote URL 
     ```
### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 9. Push the changes to your reposirtory.
   - ```
      git push origin main
      #pushes the commits to the remote repository in the branch named 'main'
     ```

<br>
<br>

###  &nbsp;&nbsp; b.) Getting the latest updates from the repository
   - b.1) just getting the updates
      - b.1.1) to straight up get all the changes from the remote repo
         ```
            git pull origin branch-name
         ```
      - b.1.2) to check/compare first, the changes since last pull/commit/update, before executing git pull
         ```
            git fetch origin branch-name
            git diff branch-name
            #after checking, and everythings seems fine, execute pull
            git pull origin branch-name
         ```
   - b.2) updating local repo after a merge commit
      - b.2.1) update main branch in local repository
         ```
            git pull origin main
         ```
      - b.2.2) update the other branche that participated in merge commit
         ```
            git pull origin branch-name
         ```
      - b.2.3) checkout / switch to the other branch
         ```
            git checkout branch-name
         ```
      - b.2.4) merge the other branch with main
         ```
            git merge main
         ```
      - b.2.5) push to remote repo
         ```
            git push origin branch-name
         ```