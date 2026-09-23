## Difference between Git and GitHub?

GitHub is where we store our repository, it is not a replacement for Git. GitHub is also used to access the repository from other computers on the cloud. In short, Git is used for management of repository and GitHub is used to store the repository.

For Git:
1. Version Control System (Snapshots of versions).
2. It is a local directory, so we can use it while being offline.
3. It is distributed i.e. it can exist on many different computers.

For GitHub:
1. Uses Git (copies or clones the repository).
2. It is always used online.
3. It adds user management, it is the place where many users collaborate and share the same repository and work on it.
4. It also allows tool integration, for instance we can use Slack for getting notified when two branches merge or report a bug or there is a new version etc.

## Commands

1. git remote add origin [GITHUB_LINK]  
   Connects your local repository to the GitHub repository.

2. git push origin master  
   Pushes your local specified branch (here master) and its commits to GitHub.

When we update the repository directly from GitHub, our local repository becomes outdated and we need to pull new commits from GitHub.

Use following commands:

First, git branch --set-upstream-to=origin/master master  
Links the local master branch to the remote origin/master branch.

Then, git pull  
Fetches and merges the latest changes from the remote branch into the local branch.

## For tracking the changes

Use commands:

git fetch  
Downloads the latest changes from the remote repository without merging them.

git status  
Shows the current state of your working directory and branch like how much commits this local repository is behind or ahead, if there are any local changes that are not staged for commit or changes that are not yet committed etc.

git pull  
Fetches and merges the latest changes from the remote repository.
