

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

### Author and Contributors

An author is the person who wrote an article, a contributor is everybody else who made modifications or extensions.