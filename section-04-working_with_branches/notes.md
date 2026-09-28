## Good Practices of Version Control

We should add new code in a way in which we can ensure that atleast one working version is there.

So we should work with branches like `master` will contain the working version and while adding new features we will create branches.

We have `test` branch and only when we are certain we send the changes to `master` branch.

We have `dev` branch in which developer directly pushes the code and this changes are sent to `test` branches for testing.

## What is a Branch?

A branch in GitHub is a separate version of a repository where you can work on changes without affecting the main code.

## Pull Request:
A Pull Request is used to request that changes from one branch be merged into another branch.

It is commonly used when:
- Working on someone else's repository
- Collaborating with a team
- The target branch is protected and requires a PR

If we have permission and the branch is not protected, we can merge a branch directly without creating a Pull Request.

## Commands for creating and working with branches

1\. `git branch <NAME>`

   Creates a new branch with the given name.

2\. `git checkout <NAME>`

   Switches to the specified branch.

3\. `git checkout -b <NAME>`

   Creates a new branch and switches to it.

4\. `git branch -d <NAME>`

   Deletes the specified branch.

5\. `git checkout --track origin/test`

   Creates a new local test branch that tracks the remote origin/test branch.

6\. `git log --graph`

   Displays the commit history as a text-based graph showing branches and merges.

7\. `git merge branch1 branch2`

   First go into that branch which is branch2 then execute merge command this will merge the branches into one, then also remove branch1 for good practices.

## Gitingore
When there are files which contain sensitive information or some information which we don't want to share we include name of these files in this file and they won't be pushed into github.

There can be multiple .gitingore files accross different folders in local repository.

Format for particular file: /filename 
Format for whole folder : foldername/
Format for particular extension files inside folder : foldername/*.txt