# Creating your first local repository

Folders and files are not version-controlled until we explicitly ask them to be. This process is called **initialising a repository**.

Firstly we need to create a folder to hold our files. We do this at the git command prompt using the following syntax:

	mkdir -p gitrepositories/foss4gukdontbeafraid

This creates a folder called gitrepositories and a sub-folder called foss4gukdontbeafraid in one step. 

**Where is this?**

If you don't specify a location for this folder, then it will use a default location as follows:

 * Linux: /home/yourname
 * Windows using Git Bash: C:\Users\yourname
 * Windows using GitHub Desktop: C:\Users\yourname\Documents\GitHub
 * Mac using Git from XCode: /Users/yourname
 * Mac using GitHub Desktop: 


Now change directory to foss4gukdontbeafraid:

	cd gitrepositories/foss4gukdontbeafraid

Initialise it as a repository:

	git init

This might not appear to do anything but it creates a hidden folder called .git inside foss4gukdontbeafraid that contains the information Git needs to track your repository.

**On windows, change your folder preferences to "always view hidden folders" so you can see this folder**

That's all we can do until we start adding some files and making changes to them, so let's make a file:

	touch blah.txt

This creates a blank text file called "blah.txt" in the folder.

At this point, we have enough in place to start committing to our repository.


