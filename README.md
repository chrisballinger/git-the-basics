# Git and Github: What You Should Know

© 2013, Chris Ballinger. License: [CC BY-NC-SA 3.0 US](http://creativecommons.org/licenses/by-nc-sa/3.0/us/)

# Git

## Version Control
* Track your changes.* Experiment without sacrificing stability.* Quickly revert unworkable code.* Prevent data loss.
## Why Git?
* It’s fast.* It has painless branching and merging.* It’s distributed (you can make commits offline).* **GitHub.**
## The Basics
* `$ git init`	* The first step to tracking your changes.* `$ git add .`
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

* Free for open source.* Diff viewer.* Network graph.* Large open source community.* Forks / Pull requests.
## Open Sourcing Your Code
* **Important:** Make sure you **NEVER** check in secrets to your git repository. (API keys, passwords, private keys, etc)* When you accidentally commit a password and push it to a public remote, consider it out in the open permanently.	* **Change the password!** * You can avoid this by using a `‘.gitignore’` file.	* Place this in the root of your repo and fill it with file names and directories you wish to ignore.	* It can also be helpful to avoid clutter (for example .DS_Store files on OS X)
## Choose a License
* **Permissive**: MIT, BSD, Apache 2.0	* TL;DR: People can use your code and create closed-source forks commercial forks of it, just by attributing you.	* These are gaining in popularity because they are frequently seen as more “commercially friendly”.* **Copyleft**: LGPL, GPL, AGPL	* LGPL: Commonly used for libraries. More permissive than GPL, allows keeping code “linking” to the library closed. (Example: ffmpeg)	* GPL: Requires people distributing binaries of your code to also provide the source code. It is also “viral” in that any code linked with GPL’d code must also be licensed under the GPL. (Example: Linux)	* AGPL: Like the GPL, but requires source distribution when running the software over a network. (Example: MongoDB)
## Don’t forget a README
* README files are extremely important. This is the first thing that people will see when they visit your repository.* They should address the following concerns:	* What is this project?	* Who wrote it? What is the license?	* How do I set it up / get it running / use it?	* Documentation	* **How should I contribute back my improvements?**
## Forks
* When using someone else’s code, it’s often a good idea to fork their code if you plan on making changes or improvements.* You will show up in the Network graph so other people can find your improvements.* It will make it easier to submit pull requests to the upstream project.* **Advanced**: When including libraries in your project, if you add the fork as a **submodule** you can track the changes of the two projects separately.
## Pull Requests* After you’ve made some changes to your fork, you would like to see your changes merged back into the original project.* Be descriptive about the changes you have made in the Title and Description.* **Pro Tip**: Create a feature branch for your pull request.
## Why Develop in the Open* You may find other people using your code in creative, original ways.* People might submit pull requests to fix bugs or add features.* Your entire platform is probably built on open source software. Give back!* Designing parts of your platform for “public consumption” can result in **better documentation** and **code quality**.## Thank you!
[Follow me on Github!](https://github.com/chrisballinger)[OpenWatch on Github](https://github.com/OpenWatch)