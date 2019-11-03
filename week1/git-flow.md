# Git flow

This quick guide was ripped direct from the README for our ![first project](https://github.com/fac18/dynamyk-site): 

Mastering git flow was a key problem we had to manage.

So that we never forget, we'll distil it here for all to see!

The quote blocks represent activity outside of the command line (probably on our project on VS Code or Atom, or on the GitHub repo itself).

So, assuming you've already `git clone`'d the repo sometime in the past, and you've already navigated to the appropriate working directory, the full cycle is as follows:

```bash
git checkout master
git pull origin master
git checkout -b new-branch
```

> build the feature or making the edits for the new-branch

```bash
git add .
git commit -m 'description of changes made'
git checkout master
git pull
git checkout new-branch
git merge master
```

> resolve conflicts emerging from the merge, if any

```bash
git commit -m 'resolved conflicts from merge'
git push origin new-branch
```

> make pull request on GitHub comparing master with new-branch
> wait for team to approve (or request amendments to and resolve) the pull request

```bash
git checkout master
git pull origin master
```

Now your new-branch has been folded in to the master branch, and your spangly new feature is available to everyone, without ruining anyone elses day with a 2 hour code merge ;)

![the reality of merging](https://media.giphy.com/media/cFkiFMDg3iFoI/giphy.gif)

NB. Obviously all these commands would in practice be regularly interspersed with the one and only `git status` to really get a handle on the position of the _HEAD_, relationship to most recent origin/master pull, the state of working directory versus the staging area, etc.
