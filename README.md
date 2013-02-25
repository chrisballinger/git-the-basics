# Git and Github: What You Should Know

© 2013, Chris Ballinger. License: [CC BY-NC-SA 3.0 US](http://creativecommons.org/licenses/by-nc-sa/3.0/us/)

# Git

## Version Control
* Track your changes.




	* Track all files in this directory.
* `$ git commit -m "First commit"`
	* Make your first commit.

## Adding Remotes

* `$ git remote add origin git@github.com:user/repo.git`
	* Set a remote URL for your repository.
* `$ git push origin master`
	* Push your changes to Github.
* `$ git remote add bitbucket git@bitbucket.org:user/repo.git`
	* Set another remote URL for your repository.
* `$ git push bitbucket master`
	* Push your changes to Bitbucket.
	
## The Usual Workflow

* `$ git add .`
* `$ git commit -m "Added some stuff"`
* `$ git push origin master`

This is all you need in order to use the basics.

## Branching and Merging

* `$ git branch`
	* Check your current working branch.
* `$ git fetch`
	* Fetch any remote branches you are tracking.
* `$ git merge origin/master`
	* Merge changes in origin’s copy of the master branch into your current working branch.
* `$ git pull origin master`
	* Essentially shorthand for git fetch & git merge origin/master.
* `$ git checkout -b branchname`
	* Make a new branch off of whatever branch you’re on.
* $ *commit some stuff*
* `$ git push origin branchname`
	* Push your changes to that branch to origin.
* `$ git checkout master`
	* Switch back to the master branch.
* `$ git merge branchname`
	* Merge the commits in branchname into master.
	
## Advanced Usage

For a more comprehensive guide and other resources: http://git-scm.com/doc

# Github

## Why It’s Awesome

* Free for open source.










