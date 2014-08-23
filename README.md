Gitting Started
===============

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

3) *I want to see what I've changed*
```
git status
```

4) *I want to commit my changes and start a code review*

Add all changes to the commit, execute the commit, then push TO YOUR FEATURE BRANCH
```
git add .
git commit -m 'I made my_cool_feature'
git push origin/my_cool_feature
```
Then follow [github's instructions for creating a pull request](https://help.github.com/articles/using-pull-requests#shared-repository-model)