_Summary:_
Git is a version control tool that lets you make changes to your code by keeping track of incremental changes to your project along the way. Git can operate locally on your own machine or it can be part of a distributed version control system such as GitHub. GitHub provides a central place for you to store and reference your code, making it very convenient for collaboration. Projects on GitHub are called "repopsitories." You add code to a repo by making a commit and pushing to it. You can retrieve code from GitHub by pulling changes or cloning a repository. To work on a collaborative project, you can fork the repository and create your own branch, which will then be compared to the master branch and either merged in or amended. You can ask the owner of the project to merge your branch by intiating a pull request. Create an account by going to [github.com](https://github.com/).

_Tips:_

* Don't commit code that doesn't work to the master branch. You can always check what branch you are on by typing `git branch`.
* Before you resume work on a project you've worked on before, type `git pull` in your terminal to get the most recent version of the document.
* Merge conflicts happen if multiple collaborators edit the same portion of a file. Make sure you [examine any conflicts before merging](https://help.github.com/articles/resolving-a-merge-conflict-from-the-command-line) the branch in question.
* If you're working with other people, don't assume that someone else is in charge! All team members should be aware of what's being merged into the master branch.
* You can avoid tracking certain changes by creating a `.gitignore` file. 

_Resources:_

1. [GitHub First Steps](https://guides.github.com/introduction/desktop/)
by GitHub Guides

* GitHub desktop (for Mac or Windows) is a really easy way to get started using git and GitHub.com.
* Here's how to create a new repository: https://help.github.com/articles/creating-a-new-repository (To do this from the commandline you can type `git init` and then add files to the newly created empty repository by typing `git add`.)
* [GitHub's YouTube channel](https://www.youtube.com/user/GitHubGuides) provides a number of training videos you can watch if you are a visual learner.

2. [GitHub Cheatsheet](/assets/github-git-cheat-sheet.pdf)
by GitHub Training

* Outlines steps for getting started with git, from installation to use.
* Serves as a reference for common commands
* To try out commands in an interactive environment, visit [Try Git](https://try.github.io/levels/1/challenges/1)
* The official git reference provides [an even more exhaustive list of commands](http://gitref.org/)

3. [Understanding the GitHub Workflow](https://guides.github.com/introduction/flow/)
by GitHub Guides
last update December 12, 2013

* Create a branch of the project you want to work on. This is a good idea even if it's your own repository. The `master` branch should *ALWAYS* be deployable.
* Add commits as you get to finite points in your code (i.e. a feature is complete and you know it works). Make sure you write explanatory commit messages along with your commits. Commits provide checkpoints to which you can rollback if need be.
* Open a pull request; discuss your code!
* Merge and deploy!
* For more documents like this, explaining specific steps for specific things you want to do on GitHub, check out the [GitHub Guides](https://guides.github.com/).

4. [Undo Mistakes Using Git](http://bytesizedthoughts.com/git/2014/05/21/git-undo-by-example/)
by bytesizedthoughts
published May 21, 2014

* The first rule of thumb is to maintain a clean working copy by committing early and often! Whenever something works, make a commit.
* Using the `--force` command is usually not a good idea. If a command won't run and you have to force it, it's likely that you're doing something wrong.
* `git reset file.txt` unstages a commit that has not been pushed
* `git commit --amend -m 'correct message'` changes your commit message
* Rebasing is a good option if you have multiple commits that need to be altered
* `git revert commitnumber` undoes a pushed commit
* There's a certain time and place for the several different undo options in git.

5. [Gists](https://help.github.com/articles/creating-gists)
by GitHub Help

* Gists are an easy way to share snippets of code.
* They have all the functionality of a git repository (i.e. forking, cloning, etc.).
* You can provide the URL of your gist to someone else so that they can view the code or text.
