# git
Generally we should think a git project is made up of three folders or directories:
1- Working directory: Any changes made without saving, tracking or adding to stagging directory.
2- Staging area or staging directory: Here we added our changes from previous stage: modifying files contents, adding new files to our repo.
3- Repository or remote directory: Here is what we have pushed to remote server through other teams or colleagues can pull our projects.
Working directory --> Staging area --> Repository

First we should install git to our work station by typing the following command.
$ sudo apt-get install git
To check git installation, you should type the following command: 
$ git --version

Later, let us suppose there is a remote repo we want to pull and contribute in it.
So First we should clone it to our local by typing the following command: 
$ git clone https://repo_url

To see git logs, you could type:
$ git log
The result shows the users (User's email,  name and commit's message) who 
have contributed to the repo chronogically.

To check whether there are changes in your working directory or not, you 
could type the following command:
$ git status
the result generally is divided into two parts
The first part and colored in green means you added the corresponding files which
have modifications you made to the staging directory (they have been mnoved from
your working directory into the staging directory). these files need to be commited and pushing later.
The second part and in generally colored in red means you either removed them 
from tracking or didn't added yet them to the stagging directory.
************************************************************************
************************************************************************

In case you want to revert all your changes and clean the working 
directory, you should type the following command:
$ git reset --hard
 
************************************************************************
************************************************************************

To list local branches, type the following command:
$ git branch
But in order to list all branches local and remote, type the following 
command:
$ git branch -a


************************************************************************
************************************************************************ 
 
To switch to another branch, type the following command:
$ git checkout branch_name

************************************************************************
************************************************************************

To create new branch in your local, type the following command
$ git checkout -b new_branch_name

BUT in this case, it is better to push your new local branch to remote server
by type the following command:
$ git push -u origin your_local_branch_name
AND in this case your local branch is set up to the remote branch 

***********************************************************************
*********************************************************************** 



  
