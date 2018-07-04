Github is a version control software.
It is widely used among developers, 
	to open source their projects, 
	to maintain and track multiple versions of their projects,etc.,
Infact, github can be used to showcase your projects and used as your new Resume.

Github was recently bought by Microsoft for $ 7.5Million!!!!

Following are some of the commands that'll get you started with github,

But first, Go to "https://git-scm.com/downloads" and download & install the latest version of git on your computer. Open your control panel and try out the following commands,


# Gives back the username of the user
$ git config --global user.name

# To set the username
$ git config --global user.name "Your username"

# Gives back user's email linked to the github 
$ git config --global user.email

# To set your email 
$ git config --global user.email "your_email_id@abc.com"

# To set color to your git in order to easily deal with commits and changes without confusion
$ git config --global color.ui true

# To list out all the global settings linked with your git, just type
$ git config --list

# To get documentation about any git command, 
$ git help git_command

## Example::	$ git help config

# Now, To initialize a git repository, 
# Go to your project folder and type in 
$ git init
# This will create a .git folder in your repository that'll maintain all the information about your commits and changes

# After you have made any changes to your Repository, you need to add your changes to the "Staging Area", by typing in
$ git add filename  
# This adds the file that you have specified to the staging area

$ git add .
# adds all the files(on which changes have been made) to the staging area

$ git add -A
# adds all the files to the staging area

$ git add -p
# lists out the file changes one my one and asks the user whether to stage the change or not

# What if you staged some change by mistake and you want to unstage it, 
$ git reset file
# This command unstages the 'file' from the staging area

$ git reset
# This command unstages everything from the staging area

# After the changes are staged, all we need to do is commit those changes
# In order to commit the changes made in our repository, type the command,
$ git commit -m "Some message describing the changes that have been made in the repo"

# if you are not sure if all the files that were modified are commited, you can check the status of your repository by using the command, 
$ git status
# This command gives the status of your repo, 
# 	whether there are any file changes that need to be staged, or
#	there are new files added to the repository but are not yet commited, or
#	there are no changes made to the repository

# Say you are working on some big project and you ended up making so many commits on your repo that you lost track of it, 
# In such a case, you can just type in, 
$ git log
# This command gives all the information about your past commits, time of commit, author who made the commit and the unique hash value of each commit.

# If you just need the list of past commits and nothing else, you could use
$ git log --oneline

# Say you have a folder which is contains personal details or you dont want that to be considered for staging,
# What you could do is, 
# create a .gitignore file and open it
# enter the name of the file that you want git to ignore
# save the gitignore file and exit
# now try running git status command , and you can see that git no longer considers that file for staging

## Until now we saw how to commit changes to our local Repo
# Lets see how to clone remote Repositories and push our local repositories to remote repos

# To clone a remote repo, 
$ git clone <url_of_the_remote_repo> location_to_clone

# Once cloned, you can view the status of the remote repo by using, 
$ git remote -v

# To view info abt branches in both remote and locally cloned repo, 
$ git branch -a

## After making any changes to local repo, to push it into the remote repo, 

$ git diff
# Shows the changes made to the local repo

$ git add .
$ git commit -m "message"

# Pushing to the remote repo, 
$ git pull origin master
# This command will pull any changes that have been made till the last time we pulled from the repository

$ git push origin master
# Pushes the local repository to remote repository

# To list out all the branches
$ git branch

# To create a branch
$ git branch branchA

# To switch to branchA
$ git checkout branchA

# To push branchA to remote Repository
$ git push -u origin branchA

# To check remote branch status
$ git branch -a

# To list all the merges that have been performed
$ git branch --merged

# To merge branchA to master
$ git checkout master
$ git pull origin master
$ git branch --merged
$ git branch merge branchA
$ git push origin master

# To delete branchA
$ git branch -d branchA
$ git branch -a
$ git push origin --delete branchA
# This deletes branchA from the remote repository too



