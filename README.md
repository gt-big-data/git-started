Gitting Started
===============

(NOTE: This documentation is a work in progress. Feel free to start an issue with it and send a pull request through github to fix the issue)

## Why?
- Git lets us all contribute features at the same time without a lot of frustrations.


## Configuring git
We'll isolate our change sets by pushing our change sets to their own feature branches. For this reason, it's convenient to automatically allow git to create
a branch of the same name as your local one on the server.
```
git config --global push.default current
```

## Cheatsheet
This will serve as a commands cheat sheet for common situations. All these assume you're in a valid git repo

1) *I want to get all the code from repo X onto my machine*
```
git clone https://github.com/gt-big-data/X.git
```

2) *I want to create a new feature/fix a bug/refactor some code (solve an issue)*

Switch to the local repo, then make a new feature branch.
```
git checkout -b my_cool_feature
```

3) *I want to see what I've changed, I want to see what branch I'm on, or I want to know if my merge was successful*
```
git status
```

Git log will also show your latest commits
```
git log
```

Git diff will show you exactly what you've changed
```
git diff
```

4) *I want to commit my changes and start a code review*

Add all changes to the commit, execute the commit, then push TO YOUR FEATURE BRANCH
```
git add .
git commit -m 'I made my_cool_feature'
git push origin my_cool_feature
```
Then follow [github's instructions for creating a pull request](https://help.github.com/articles/using-pull-requests#shared-repository-model)

If you are denied access, please [create an issue](https://github.com/gt-big-data/git-started/issues/new) and gt-big-data admins will give you push access to all repos.

If you have push access, you will be able to merge other people's pull requests. Try not to merge your own pull requests.

If github says you can't "automatically merge this pull request," then the owner of the pull request needs to get the latest changes from master, and push those changes to their feature branch.

5) *I need to get the latest changes from master*
```
git pull origin master
```
If there's a conflict, see [git scm section on conflicts](http://git-scm.com/book/en/Git-Branching-Basic-Branching-and-Merging#Basic-Merge-Conflicts).

Note: since we're all pushing to NAMES.md, there may be conflicts.

## Git Resources
Here's a list of pretty good git resources. Feel free to add in a pull request.

1) [try.github.com](http://try.github.io) is a fun, interactive, and dynamic basic tutorial to Git commands via the command line.

2) [Understanding Github: a journey for beginners](http://readwrite.com/2013/09/30/understanding-github-a-journey-for-beginners-part-1) and it's following articles (part 2, etc.) offer a more comprehensive and detailed guide to Git commands, terms, and workfows.

3) [Learn git branching](https://pcottle.github.io/learnGitBranching/?demo) is a good playground for visualizing what's going on when you execute git commands. When you feel confident enough, you can go into [interactive mode](https://pcottle.github.io/learnGitBranching/)

4) [Git Tutorial (from atlassian)](https://www.atlassian.com/git/tutorial) is good for learning about all the different commands. [Git Basics](https://www.atlassian.com/git/tutorial/git-basics) and [Git Branches](https://www.atlassian.com/git/tutorial/git-branches) are good starting points.
