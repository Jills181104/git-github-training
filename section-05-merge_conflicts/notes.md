## When merge conflict occur?

A merge conflict occurs when Git cannot automatically combine changes from two branches, usually because the same part of a file was changed differently in both branches.

Conflict does not occur when different branch works in different file and even for same file if both updated same file but they updated different line of code then also git will be able to merge without conflict. 

## Merge types

1. `Fast Forward merge`

    Moves the current branch pointer forward to the latest commit of the other branch when there are no new commits on the current branch.

2. `Recursive merge`

    Combines two branches by finding their common ancestor and creating a new merge commit when needed.

## Commands learned

1. `git merge --abort`
    Cancels the current merge and restores the repository to its state before the merge.

2. `git tag -a v1.0 -m "MSG"`
    Creates an annotated tag named v1.0 with a message.

3. `git log --pretty=oneline`
    Displays each commit in a single line.

4. `git tag -a beta HASH_VALUE -m "MSG"`
    Creates an annotated beta tag on the specified commit.

5. `git push origin --tags`
    Pushes all local tags to the remote repository origin.

>Note : When we are doing git pull or git push we are acutally merging from remote branch to local branch and vise versa.