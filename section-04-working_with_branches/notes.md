## Good Practices of Version Control

We should add new code in a way in which we can ensure that atleast one working version is there.

So we should work with branches like `master` will contain the working version and while adding new features we will create branches.

We have `test` branch and only when we are certain we send the changes to `master` branch.

We have `dev` branch in which developer directly pushes the code and this changes are sent to `test` branches for testing.

## What is a Branch?

A branch in GitHub is a separate version of a repository where you can work on changes without affecting the main code.

## Commands for creating and working with branches

1\. `git branch <NAME>`

   Creates a new branch with the given name.

2\. `git checkout <NAME>`

   Switches to the specified branch.

3\. `git checkout -b <NAME>`

   Creates a new branch and switches to it.

4\. `git branch -d <NAME>`

   Deletes the specified branch.