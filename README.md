Gitting Started
===============

(NOTE: This documentation is a work in progress. Feel free to start an issue with it and send a pull request through github to fix the issue)

## Why?
- Git lets us all contribute features at the same time without a lot of frustrations.

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
git push origin/my_cool_feature
```
Then follow [github's instructions for creating a pull request](https://help.github.com/articles/using-pull-requests#shared-repository-model)

If you are denied access, please [create an issue](https://github.com/gt-big-data/git-started/issues/new) and gt-big-data admins will give you push access to all repos.


5) *I need to get the newest changes from master*

```
git checkout master
git pull origin/master
```
If there's a conflict, see [git scm section on conflicts](http://git-scm.com/book/en/Git-Branching-Basic-Branching-and-Merging#Basic-Merge-Conflicts)