# Forking Workflow

## Starting to Work on a Project

1. Go to the GitHub repository.
1. Click the "Fork" link in the upper right to create a forked repository.
1. Go to your GitHub repositories view, and copy the URL to the forked repository.
1. In SourceTree, clone your forked repository using the URL.
1. Go to the original repository in GitHub and copy the clone URL.
1. In SourceTree, add a new remote called "upstream" using the original repository
  clone URL.

## Getting Ready to Do Work on a Feature

1. Fetch all changes from all remotes.
2. Switch to the master branch.
3. Pull any changes from upstream/master to the local master so that it matches the tip of upstream/master.
4. If origin/master is now behind the local master, push to origin/master. At this point the local master, origin/master, and upstream/master should match.
5. Create a branch for the new feature.

## Working on a Feature

1. Edit files.
2. Stage changed files.
3. Commit changes locally. Do not push to the remotes.

## Pushing Changes to a Feature

It's best if the changes are rebased to the tip to keep the history as linear as possible.

