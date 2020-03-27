

# Github

## Why use Github
The beauty of Git and Github is collaboration and version control.
- Use this to track the history of a project
- Allows multiple people to work on the same project at once

### Git vs. Github

- Git
	- The actual version control software
- Github
	- Web service for git projects
	- Like a social media for a git project

## Key Terms

- Repository
	- Repo for short
	- This is where you will be storing everything for the project
- Commit
	- Think of this like saving
	- Add messages to your commits to explain what you're committing
	- You can browse the history of each commit and see what was changed
- Branches
	- Can create different code bases within your repo
	- Think of it almost as a different save as of a whole repo
- Merge
	- One branch absorbs another branch
- Fork
	- Like taking a whole repo, and creating a new instance of that under your own account
	- You now will have an exact replica of that repo, including it's history
	- We can then make as many changes as we want without affecting the original repo
- Pull Request
	- If I'm happy with what I've been working on, I could create a pull request to the original repo
	- This would mean I want to add my code to the original repo
	- Then the owner of the original repo can decide whether they want to pull my changes or not
- Cloning
	- Taking a repository that's on a server, and putting a copy of it onto your own computer

## Git Commands

- git status
	- Tells you the branch you're on
	- Also tells you how your branch compares to the repo
	- Mainly tells you whether there are changes or not
- git commit -a -m "Adding something"
	- This will commit all
	- The -m with the quotes will add the quotes as the commit message
- git log
	- See your local history of commits
- git remote -v
	- This will list all of your remotes
- git remote add upstream https://github.com/erikstacy/Notes.git
	- This adds a new remote called upstream to the linked repo
- git push origin master
	- **origin:** The remote you want to push to
	- **master:** The branch you want to push to
- git branch
	- Lists all of the branches
- git branch -a
	- Lists all branches local and remote
- git branch newbranch
	- Creates a new branch named newbranch
- git branch -d newbranch
	- Deleted newbranch
- git checkout master
	- Switch to branch master
- git fetch upstream
	- This will fetch everything from the upstream remote repo

## Issues

This is purely a Github concept.
- Helps with collaboration in a repo
- Components
	- Title
	- Body with a description
	- Labels
		- Helps to give a quick understanding of the issue
	- Milestone
	- Assign
		- If you need someone specifically to work on this
- Open Issue
	- Means the issue still exists and is being worked on
- Closed Issue
	- The issue has been resolved
	- Only the person that opened the issue or the owner of the repo can close an issue
- All issues have an ID number
	- When making a commit, you can put the ID number in the commit title to link this commit to the issue
	- So if the issue is #10, you could put #10 in the commit title and it will show up under the issue
- There are certain key words in a commit that will close an issue
	- If you put the word "fixes" within the commit title with the issue ID, it will close that issue
- We can also reference commits within an issue
	- Pasting a commits hash code into the description of an issue will link to that commit

## Github Pages

- gh-pages
	- The name of your "master" branch
	- Can work just like your master, but will automatically make a url that anyone can access
	- Make this the default branch
		- Settings, branches
		- Default branch can be changed here
	- At this point we can delete the master branch
- index.html
	- This will be the defualt page when you go to the url

## Resolving Merge Conflicts

- When two people make a change to the same line, a conflict happens
- We can pick which line gets to actually be added
- Could leave this up to the contributor that caused the conflict, or resolve it yourself
- Once the conflict is resolved, we can merge the pull request

## Remotes

- Different instances of the repo
- You can make different remotes from other people's forks of repo so you can merge their code into yours

### Author and Contributors

An author is the person who wrote an article, a contributor is everybody else who made modifications or extensions.

# Contributing to Open Source projects

- Before you do anything, check the CONTRIBUTING.md file to see how that project wants you to go about doing things
- Typically you would open an issue when you want to make a contribution
	- Write in detail what it is that you want to contribute
	- Eventually the maintainer will respond, maybe with a question, or saying to go ahead
- Once you get the go ahead, double check CONTRIBUTING.md just to check if there's a way they want you to set things up
- BEFORE MAKING CHANGES, MAKE SURE THE INITIAL CLONE WILL BUILD AND RUN
- When you fork and clone the project, you have now made your own project completely on it's own different track
	- The upstream repository could get a bunch of commits, but yours will not
	- If we want to keep up to date with upstream repository, we must take some steps
		- Go to the upstream repository and create a new remote for that
		- At this point you should have one remote for your personal fork repo, and one remote for the upstream repo
		- Make sure to fetch the upstream remote into your master so we have up to date code
		- We want our master to be pointing to the upstream repo so that it's up to date with the open source code
			- Here's the trick
			- git branch --set-upstream-to=upstream/master master
		- Now when we pull on our master branch, we're pulling from the upstream repo
	- We then want to make our branches off of this new master