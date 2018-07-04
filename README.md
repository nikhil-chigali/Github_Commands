Github is a version control software.
It is widely used among developers, 
	to open source their projects, 
	to maintain and track multiple versions of their projects,etc.,
Infact, github can be used to showcase your projects and used as your new Resume.

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
# ------------

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
# This command gives all the information about your past commits, time of commit, author, etc.,

# If you just need the list of past commits and nothing else, you could use
$ git log --oneline



