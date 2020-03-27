
# WHO Flutter App

[Github Link](https://github.com/WorldHealthOrganization/app/blob/master/docs/ONBOARDING.md)

## Goals for the v1.0

Read more [HERE](https://github.com/WorldHealthOrganization/app/blob/master/docs/ROADMAP.md)

**Target Date:** March 30, 2020

**Goal:**
- Native look and feel
- Dynamically updatable port of the WhatsApp bot content
- Information able to be given to specific country and language
- Ability to push notifications in the future

## Questions To Answer

- What is a committer, and would I be a committer?
	- If so, I need a hardware key

### Rules

- Enable 2FA for github account
	- Hardware key mandatory if you are a committer
- Assign issues to yourself in github
	- Do this before working on code
	- This is to avoid duplicate effort
	- If someone already has the issue, sync up before-hand
- Assign PRs to people whose approval I need
- Assign the issue or PR to anyone who is blocking you
	- Be bold
- PRs assigned to you are high priority

### Pull Requests

- Authors, before submitting a PR for review
	- Add your name to the end of the team array [here](https://github.com/WorldHealthOrganization/app/blob/master/content/credits.yaml)
	- Make sure commit history is only important chunks
		- Squash smaller changes that were distributed through multiple commits into one large commit
		- Organize these larger commits to reflect meaningful chunks of changes
		- Example of this is a code review coming back with corrections needed. Once those changes are made are re-commited, this new commit should be squashed into the previous commit
	- Github email address must match git author email address
	- All dependancies that you add must be acknowlodged in PR description
		- Describe why you chose it
		- Show it's license
		- Summary of how widely it is used in open source community
			- Does it have known apps using it?
			- Are there known backers?
- Committers
	- 2 person rule
		- Code can only be committed with approval of one other person with commit authority
	- Committers must use Squash and Merge function for merging a PR

### Commit Message Guidelines

If you need this, here's the [link](https://github.com/WorldHealthOrganization/app/blob/master/docs/CONTRIBUTING.md), scroll to the bottom.