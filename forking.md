# Forking Workflow

## Starting to Work on a Project

1. Go to the GitHub repository.
1. Click the "Fork" link in the upper right to create a forked repository.
1. Go to your GitHub repositories view, and copy the URL to the forked repository.
1. In SourceTree, clone your forked repository using the URL.
1. Go to the original repository in GitHub and copy the clone URL.
1. In SourceTree, add a new remote called "upstream" using the original repository
  clone URL.
1. Fetch changes from all remotes.
1. Right-click on the master branch, and select Track Remote Branch > upstream/master, and click OK when asked to confirm.

At this point your local master and upstream/master should be on the same commit. That's the state we want to keep the local master in.

We can let origin/master languish, since we will never generate pull requests from that branch. However, you can always update origin/master like this:

1. Switch to the master branch.
2. Click the Push button and select to push master to the origin/master branch.

At that point, four branches should be side-by-side on the same commit: upstream/master, origin/master, origin/HEAD, and the local master. Again, that's optional (but looks very clean).

## Making the Local Master Match upstream/master

Periodically you will have to update your local master to match upstream/master. Do that as follows:

1. Fetch changes from all remotes.
2. Switch to the master branch.
3. Click the Pull button and pull from origin/master. Since you are not making any direct changes to the local master, this should not produce any conflicts.

At this point the local master and upstream/master should be on the same commit.

## Getting Ready to Do Work on a Feature

1. Make sure your local master matches upstream/master, as described above.
5. Create a branch for the new feature.

## Working on a Feature

1. Edit files.
2. Stage changed files.
3. Commit changes locally. Do not push to the remotes.

## Pushing Changes to a Feature

It's best if the changes are rebased to the tip to keep the history as linear as possible.

1. Make sure your local master is up-to-date with upstream/master, as described above.
1. Switch to the feature branch.
1. Rebase and fix any conflicts. Use Actions > Continue Rebase if there were conflicts, do not commit.
1. Commit any changes necessary to fix the conflicts.
1. Create a pull request from the feature branch using these parameters:

Submit via remote: origin: https://www.github.com
Local branch: the name of the feature branch
Remote branch: the name of the feature branch

The first time you commit, you will be asked to enter your name and email address, if you haven't already configured them in SourceTree preferences.
