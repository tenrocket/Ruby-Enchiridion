
1. [GitHub Cheatsheet](/assets/github-git-cheat-sheet.pdf)
by GitHub Training

* Outlines steps for getting started with git, from installation to use.
* Serves as a reference for common commands


2. [Understanding the GitHub Workflow](https://guides.github.com/introduction/flow/)
by GitHub Guides
last update December 12, 2013

* Create a branch of the project you want to work on. This is a good idea even if it's your own repository. The `master` branch should *ALWAYS* be deployable.
* Add commits as you get to finite points in your code (i.e. a feature is complete and you know it works). Make sure you write explanatory commit messages along with your commits. Commits provide checkpoints to which you can rollback if need be.
* Open a pull request; discuss your code!
* Merge and deploy!

3. [Undo Mistakes Using Git](http://bytesizedthoughts.com/git/2014/05/21/git-undo-by-example/)
by bytesizedthoughts
published May 21, 2014

* The first rule of thumb is to maintain a clean working copy by committing early and often! Whenever something works, make a commit.
* Using the `--force` command is usually not a good idea. If a command won't run and you have to force it, it's likely that you're doing something wrong.
* `git reset file.txt` unstages a commit that has not been pushed
* `git commit --amend -m 'correct message'` changes your commit message
* Rebasing is a good option if you have multiple commits that need to be altered
* `git revert commitnumber` undoes a pushed commit
* There's a certain time and place for the several different undo options in git.