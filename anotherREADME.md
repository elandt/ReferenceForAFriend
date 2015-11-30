Used With My CS 407 Team

Setup for Local Development
==============================================================================

Create a folder to hold the project

Execute a git clone to retrieve the repo

```bash
	# Make a new directory
	mkdir git
	# Navigate to Repo
	cd git
	# Clone into the repo
	git clone <enter the url for your repository here (it should end in .git)>
	# Follow rest of setup
```
Editing the files (Create your own branch)
==============================================================================

If you are making changes... MAKE SURE TO MAKE YOUR OWN BRANCH!!!

How to Create your Branch:

```bash
	# While in the Repository folder/directory and on the master branch
	git checkout master
	# Create your own branch
	git branch <Your Branch Name>
	# Checkout your branch
	git checkout <Your Branch Name>
	# Check that you are on your branch
	git status
```

How to Commit your Changes:

```bash
	# Add all the files you edit
	git add --all
	## OR ##
	git add <path to file>
	# Then commit your changes
	git commit -am "<Your message text for what changes you made>"
```

How to Merge your Changes:

```bash
	# After you commited
	# Switch back to master
	git checkout master
	# Merge your Changes (Make sure you are positive you want this!)
	git merge <Your Branch Name>
```

How to Push your Changes:

```bash
	# Push back to the Repo
	git push origin master
```

Updating your Files
==============================================================================

How to Update your 'master' branch:

```bash
	# From any branch
	git checkout master
	# Verify your in master
	git status
	# Pull in the new changes
	git pull
```

How to Update <your branch> after Updating 'master':

```bash
	# Update master first (Above)
	# Checkout your branch
	git checkout <your branch>
	# Update your branch
	git rebase master
	# Possibility to casue conflicts in the code, 
	# if you are having issues I would recommend starting
	# on a new branch from master (Details above)
```
