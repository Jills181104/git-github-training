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

## What is Rebase?

Rebase takes the commits from the current branch and reapplies them on top of another branch.

## Basic Rebase

```bash
git checkout feature
git rebase main

Replays the commits from feature on top of the latest main.

## Rebase with Remote Branch

```bash
git fetch origin
git rebase origin/main
```

Updates the current branch with the latest changes from the remote `main`.

## Rebase Conflicts

If a conflict occurs during rebase:

```bash
git status
```

Resolve the conflict, then:

```bash
git add FILE_NAME
git rebase --continue
```

### Abort Rebase

```bash
git rebase --abort
```

Cancels the rebase and returns to the previous state.

### Skip a Commit

```bash
git rebase --skip
```

Skips the commit causing the problem.

## Interactive Rebase

Used to clean up or modify recent commits.

```bash
git rebase -i HEAD~3
```

Common options:

- `pick` - Keep the commit.
- `reword` - Change the commit message.
- `edit` - Modify the commit.
- `squash` - Combine with the previous commit.
- `fixup` - Combine without keeping the commit message.
- `drop` - Remove the commit.

## Rebase vs Merge

### Merge
Merge creates a separate merge commit.

### Rebase

```text
C0 ── C1 ── C2 ── C3' ── C4'
```

Rebase creates a more linear history.

## Important Points

- Rebase changes commit history.
- Use rebase mainly on your own feature branches.
- Avoid rebasing shared branches.
- Interactive rebase is useful for cleaning up commits.
- After rebasing a previously pushed branch, use:

```bash
git push --force-with-lease
```
