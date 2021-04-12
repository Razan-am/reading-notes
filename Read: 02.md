# **Git**

### A Comprehensive Guide

......................................................................

 ***``` The contents: ```***

### **Version Control:**
   its a system that contain all the changes of a project by creating many versions depending in the number of changes of that project and provide us the ability to can revert a file or project to a previous version, track modifications and modifying individuals, and compare changes. Through it mistakes with files can easily be rectified with Version Control System (VCS).
 
**- It's divided to :**

 1. ***Centralized Version Control***: its a local version control system that entails one database on your hard disk that stores changes to files.


 2. ***Distributed Version Control*** : (DVCS) allows clients to create mirrored repositories. These data backups can be easily be placed on the server to replace any lost information. So programmers working in teams can collaborate with each other in various ways to complete a joint project.But there is amain issue about DVCS it's  the server as a single point of failure. If a CVS goes down, collaborators cannot work with each other on a file or save changes and new versions.





- So Git is ;
 ***```Git is an system that contain:```***

**Snapshots**: Git is a Distributed Version Control System  that stores data in a file system made up of snapshots of any changes you do in the projects and stores a reference to it.

**local operation**: Git relies on local operations allowing to work in any situation because a project’s history resides on the local disk and not depends on the server .

**Tracking Changes**:Any changing that applied to any file Git will be tracking it and be able to always detect file corruption or loss of information in transit.

**Loss of Data**: Becouse of how Git worked it help in minimize the possibility of irreversible damage to files, such as accidentally lost data.

**States**:Files in Git can reside in three main states: committed, modified and staged:

1. Committed :Data is securely stored in a local database

2. Modified:File has been changed but not committed to the database

3. Staged:Flagged a file’s changed version to be committed in the next snapshot

------------------------
###### ***```To start using Git you should know this upfollowing parts```***

1. You shave to download Git to you're computer

2. ***Graphical Clients***:basically its about an inherent Graphical User Interface (GUI) tools that git include it to the user, also users can use  also utilize third-party tools created for particular platforms.


3. ***Initial Customization***: After installing Git you should perform some customization steps, which should only need to be completed once on any machine:


   - Configuration of Variables:to control aspects of Git’s   operation and looks.

   - Identity Setting:users should immediately set the user   name and email address.


 **To sign it up follow these steps:**
 
   ***```Type the following into Terminal or Command Line:***```
   `< git config --global user.name "Jane Smith">`
    `<git config --global user.email "example@email.com">`

  ***```To confirm that you have the correct settings, enter the following commands :***```
   `<git config --global user.name (should return Jane Smith)>`
   `<git config --global user.email (should return example@email.com)>`

-------------------------------------------
> By using the –global option, these Git settings apply to anything on the system. To use different identity settings  for a specific project, change the working directory to the desired local Git repository and repeat the steps above without using –global.


-------------------

4. **Default Text Editor** : it is used to configure a different text editor, such as Emacs by typing  the following into your Terminal or Command Line:

 `<$ git config --global core.editor emacs>`

5. **Check Settings** :To check settings, use the To check settings, use the `<git config --list>` command.


 * Example:
 -  $ git config --list
 - user.name=Jane Smith
 - user.email=example@email.com

 6. **Getting Help** :There are three ways to get more information on a particular command, by accessing the manual:

- git help command

- git command --help

- man git-command
----------------------------------

###### ***```Setting up a Git Repository;***```

1. **Importing** :To import an existing project or directory into Git through these steps :

- Switch to the target project’s directory
Example:
`<$ cd test (cd = change directory)>`

- Use the git init command

 `<$ git init>`

-------------------
> Note: At this stage, you have created a new subdirectory named .git that has the repository files. Tracking has not commenced.

------------------------

- To start tracking these repository files, perform an initial commit by typing the following:
`<$ git add *.c>`
`<$ git add LICENSE>`
`<$ git commit -m “any message here”>`

2. **Cloning** : To create a copy of an existing Git repository from a particular server by this :

 `<$ git clone https://github.com/test>`

-----------------

 ###### ***```Workflow***```

 1. **Local Repository Structure** :The local Git repository has three components:

- Working Directory: The actual files reside here.
- Index: The area used for staging
- Head: Points to the most recent commit

2. **Saving Changes** : There is two types :
- Tracked :Tracked files can be modified, unmodified, or staged; they were part of the most recent file snapshot.
- Untracked :Untracked files were not in the last snapshot and do not currently reside in the staging area.

3. **Tracking and Staging a New File** :

* To Track:
- Single File: Track one file only by using the following format:
 `<git add filename>`

 -All Files:Track all files in a repository by using the following command:
 `<$ git add *>`

 > After using these commands, files are tracked and staged   for committing.

* For new file:After adding a new file called EXAMPLE, you would see information regarding changes to be committed when using the git status command:
`< $ git status>`

On branch master
Changes to be committed:
$ git commit -a
`<(use "git reset HEAD ..." to unstage)>`
**new file: EXAMPLE**

4. **Committing a File** :To record the changes after staging one or multiple files:
`<$ git commit -m “made change x,y,z”>`

5. **Committing All Changes** :
`<$ git commit -a>`

6. **Pushing Changes** :To  push changes to a remote repository :
- Example:
`<$ git push origin master>`
>This command pushes changes from the local “master” branch to the remote repository named “origin”.

7. **Stashing Changes** : 
-```git stash``` :This command temporarily removes changes and hides them, giving you a clean working directory. and when you want to continue working on the changes use the ```git stash apply```

-------------------------
###### ***```Remote Repositories***```

**It's provide the ability to work in versions of a project residing online or on a network on Git projects**

1. **Cloned Repositories** : Git will automatically give the name “origin” to the server from which you cloned and the name “master” to your local branch.

2. **Seeing Your Remotes** : 
-```git remote command``` you can view the short names, such as “origin,” of all specified remote handles.
-```git remote -v ``` by using it you can view all the remote URLs next to their corresponding short names.


- Example:
`<$ cd example>`
`<$ git remote -v>`
`<remote1 https://github.com/remote1/example (fetch)>`
`<remote1 https://github.com/remote1/example (push)>`
`<remote2 https://github.com/remote2/example (fetch)>`
`<remote2 https://github.com/remote2/example (push)>`
`<remote3 https://github.com/remote3/example (fetch)>`
`<remote3 https://github.com/remote3/example (push)>`



By @Jenni Choi for Udemy

**References:**
[GitHub](https://blog.udemy.com/git-tutorial-a-comprehensive-guide/)
