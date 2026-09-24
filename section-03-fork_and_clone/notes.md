# Fork

This only exists in GitHub, there is no such thing as Git Fork.

This means we can copy someone else's repository.

After forking the repository we can just clone it locally and make changes and work on it.

Then we should explore that repository.

## Commands for that task

1. `git log`  
   Shows all commits made in that repository.

2. `git diff hash_value1 hash_value2`  
   Shows what was changed between these commits.

3. `git show hash_value`  
   This not only shows details about this commit, it also shows diff of specified commit.

4. `git show HEAD~n`  
   Shows the details and changes of the commit that is n commits before the current HEAD.

5. `git show HEAD`  
   Shows the details and changes of the current (latest) commit.

6. `git show HEAD~n HEAD~n1`  
   Shows the details and changes of the commits n and n1 commits before HEAD.

## Exploring a particular file

For exploring particular file we do:

1. `git annotate file_name`  
   This lists all the changes made to that particular file over time.

## Extra commands

1. `git commit -a -m "Commit_Msg"`  
   Stages modified/deleted tracked files and commits them with the given message.

2. `git add .`  
   Stages all new and modified files in the current directory (and its subdirectories) for the next commit.

3. `git reset HEAD .`  
   Unstages all new and modified files in the current directory (and its subdirectories) for the next commit.

4. `git checkout -- .`  
   Discards the uncommitted changes and restores last committed version.

5. `git checkout hash_value <file>`  
   This will restore the specified file to the version from the given commit.

> Note: After forking the repository and we want to contribute to original repository we can create a pull request and if the owner accepts it will be shown in original repository we can see our own commit.

## Undoing changes and reverting commits

### Scenario 1 - Changes are not yet staged

`git checkout -- <file>`

### Scenario 2 - Changes are staged

`git reset HEAD file`

This will unstage the changes and we should execute again `git checkout -- <file>` for undoing the changes.

### Scenario 3 - Changes are committed

`git reset --hard HEAD~1`

This will remove the latest commit and moves HEAD by one commit.
