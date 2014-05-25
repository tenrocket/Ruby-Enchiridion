[Undo Mistakes Using Git](http://bytesizedthoughts.com/git/2014/05/21/git-undo-by-example/)
by bytesizedthoughts
published May 21, 2014

* The first rule of thumb is to maintain a clean working copy by committing early and often! Whenever something works, make a commit.
* Using the `--force` command is usually not a good idea. If a command won't run and you have to force it, it's likely that you're doing something wrong.
* `git reset file.txt` unstages a commit that has not been pushed
* `git commit --amend -m 'correct message'` changes your commit message
* Rebasing is a good option if you have multiple commits that need to be altered
* `git revert commitnumber` undoes a pushed commit
* There's a certain time and place for the several different undo options in git.