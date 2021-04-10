# GIT
---
## Web Application Development

<img src="WebApplicationDevelopment.PNG"/>

## SCM Tool GIT

<img src="SCMTool-GIT.PNG"/>

## Distributed VCS - GIT

<img src="DistributedVCS.PNG"/>

## VCS Introduction:

#### Version Control System:
- it is used to track application source code additions, modifications or deletions etc.
- history
- versions
   - version1/commit1
   - version2/commit2
   - version3/commit3

VCS --> learn as a developer (in general we never write the code)


Developers - task/work
- Developer1 --> Feature1 - userstory1
- Developer2 --> Feature2 - usersotory2
- Developer3 --> Feature3 - userstory3

#### Install and setup Git server and Client software:
1. setup a git server in two ways
 - cloud Based git server(online-internet)
 - on premises git server(install and setup git server)
       - computers (company building)

2. setup a git client
 - commandline client ( git bash )
 - gui client ( git bash gui, tortoise git)
 - web client (browser)


## GIT Architecture
---
<img src="GIT_Architecture.png"/>

#### Working On Git Repositories Using URL's

<img src="WorkingOnGitrepositoriesUsingURL.PNG"/>

## Working on GITHUB repository

**SSH key create and upload**
1. create ssh key using gitbash client
2. upload ssh key to github server

**Create a Test Repository, Download to local Repository and Upload to Remote Repository**
1. create repository "TEST" in github server
2. copy ssh url of TEST repository from github server
3. create a folder (portal) in your laptop home directory(c:/users/username) 
4. open git bash client
5. go to portal path (newly created folder - look at 3rd step)
6. use git clone command to get remote repository into local repository 
      ex: git clone git@github.com:chinnu1028/TEST.git
7. using following url go to github page and download zip file(please see the snapshot below)
8. extract or unzip the downloaded folder
9. copy and paste all the files and folders from extracted Folder(maven-project2-master) to portal directory(which is created in 3rd step)
10. git status (it shows unstaged changes) 
11. git add . (this command will add all the files and folders from working directory to staging area)
12. git status (it shows staged changes)
13. git commit -m "added files and folders" (it saves all the changes from staging to local repository)
14. git push ( it upload all added files from local repository to remote repository)
15. go to github check the TEST repository, now you see the uploaded files and directories.

#### Assignment1:
(setup git server and create remote repository, clone a copy to local repository, make some changes and push back to remote repository)

1. setup your github account(create a git server)
2. create a repository (git server)
3. install git bash (CLI client) on laptop
4. generate ssh key and copy to git server(one time task)
   - use ssh-keygen command to generate ssh key in local (laptop)
   - copy .pub key into git server (account settings - ssh keys) 
5. clone remote repository into local(git clone - ssh url)

new files:

6. create a file
7. check the file changes ( git status )
8. git add filename ( adding new file to staging area -  index file)
9. git commit -m "message" ( saving our changes to local repository - .git)
10. git push ( save local repository changes to remote repository )


existing files:

6. modify existing file
7. check the file changes ( git status )
8. git commit -am "message" ( saving our changes to local repository - .git)
9. git push ( save local repository changes to remote repository )

## GIT COMMANDS:
---
- **git clone** --> to get a copy or snapshot of complete remote repository into local (download a copy of remote repo to laptop)
- **git status** --> to see the list of files and folders which are having additions, modifications or deletions.
- **git add** --> git adds the workspace changes to staging area (it must be used for newly added files and folders)
- **git commit -a** --> git adds the workspace changes to staging area and also saves the changes from staging area to local repository ( -m option can be used for providing a message  while saving )
- **git push** --> it is used to save or upload the local repository changes to remote repository
- **git checkout** --> it is used to switch between the branches
         - **Note:** checkout command not only switch branches but also replaces the complete working directory for a branch.
- **git checkout -b branchname** --> it is used to create a new branch local.
        - **Note:** need to set upstream branch in order to push to remote repository.
- **git branch** --> it is used to create a branch locally.


## SDLC (Software Development Life Cycle )
---
![image](https://user-images.githubusercontent.com/79018042/114259647-15faf800-99ed-11eb-9561-74b669d43129.png)

![image](https://user-images.githubusercontent.com/79018042/114259679-4773c380-99ed-11eb-9c39-990419dafa97.png)

![image](https://user-images.githubusercontent.com/79018042/114259684-4fcbfe80-99ed-11eb-8a5e-070166d8ccf5.png)


client --> software company --> software product
 - requirements (Business)
 - design (system or architectural - hardware and software, 64 bit hardware, GIT, Jenkins)
 - development ( developers will write the code )
 - testing ( testers will do test and give the approval )
 - deployment ( deploying or installing application to production environment )
 - monitoring or maintainance 

Features 
 - user story1 - developer1
 - user story2 - developer2
 - user story3 - developer3

SDLC:
 - Waterfall model(traditional model) - years of time to develop an application
 - Agile Model - 3 to 6 months application to our client but not full or complete product
 - AgileDevops

Release Notes: 
 - Feature1 (enhancements)
 - Feature2
 - bug fixes

GIT:
- default branch - master/main

Remote repository and Local repository always should be in sync ( except your local changes )

## .git Directory
---
- it will track all the changes including modifications, additions, deletions etc.

![image](https://user-images.githubusercontent.com/79018042/114259753-d680db80-99ed-11eb-85cd-ffc223cfca57.png)

- **Object:** it is a memory space where object or binary code will be stored.

#### Config File Types
<img src="ConfigFiles.PNG"/>

## Application Development Using Agile Model
---
<img src="ApplicationDevelopmentUsingAgileModel.PNG"/>

## GIT Branching Strategy/Model
---
<img src="GIT_BranchingStrategy.PNG"/>

## GIT Administration
---
#### **GIT Administrator Tasks/Activities**
1. setting up Git server (creating Linux Machine and install GIT software on it)
2. creating Repositories(Remote Repository & Local Repository)
3. Access permissions to all Developers and Testers
4. Maintaining Repositories (Remote Repositories)
5. Creating Branches (Master, Release, Sprint and Feature Branches)
6. Resolving Merge Conflicts(if any)
7. Accepting Merge Requests or Pull Requests(which are created or raised by Developers)
8. Creating Tags

#### Merge Requests/Pull Requests
- Merge Requests are raised whenever one branch code needs to be merged with another branch code.
- In general, Merge Requests are raised by developers in order to get their changes into base branches from their individual branches.
- Merge requests are approved by Git Administrator for highlevel branches like master/main, release, sprint and feature branches.

- we create feature branches once development is done we merge back with release branch

Project:
- Developers
- Testers
- Devops
- Security
- Software Architecture or Infra Team

Developers:
- write the quality code
 - local repository(branch) --> push --> remote reposiotry(branch)

---
## GIT cherry-pick

<img src="cherrypick.PNG"/>

**cherry-pick**
pick one or more commits from one branch to another branch
Ex: git cherry-pick commitID

**Note:** git commit is not required for cherry-pick i.e automatically commited to required branch.

---
## Merge
merge one branch into another branch

## Merge conflicts - 3 cases
1. merging remote branch into local branch - git pull ( remote branch to local branch)
2. merging one branch into another branch ( remote repository branches)
3. merging one branch into another branch (git rebase - remote repository branches)

## Resolving merge conflicts
2 ways 
- using webclient 
- locally using tortoise git client
```
Locally:
1. git checkout Jaggu-Feature1
2. git pull
3. git checkout Feature1
4. git pull
5. git merge --no-ff "Jaggu-Feature1"
6. git push
```

## Case1

<img src="Case1.png"/>

## Case2

<img src="Case2.png"/>
