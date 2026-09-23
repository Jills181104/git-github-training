What is version control/revision control/source control?

-> It contains bunch of information about what change was made, when it was made and by whom it as made. 

Importance - Keep track of changes.
           - Ability to go back to a previous working version.
           - Easily add someone else's work into ours.

Where can i use version control?

-> Any coding files such as js, css or even doc files or pdf files.


Commands learned - 
1. git --version 
	-> for checking if the git is downloaded in system or not and also helps us find which version is in the system.

2. cd
	-> for jumping into to home directory.

3. start. 
	-> for opening the file explorer of current directory.

4. dir
	-> for listing all the files and folders in the current directory.

5. mv file_name new_file_name
	-> for renaming any file using git bash.

6. mkdir GitGithubMasterclass
	-> this creates a new folder

6. cd folder_name
	-> for change the current directory to specified folder_name

7. code folder_name
	-> for opening text editor like vscode.

8. git init
	-> for initializing empty git repository

9. git add file_name
	-> this is used for moing a specific file into Git's staging area.

10. git commit -m "message"
	-> this is used for saveing the change was previously staged.

11. git diff
	-> for reviewing the changes that are made we use this. it is very sensitive because it also tracks the new line at the end of file.

12. git config --global user.name "Your name"
	-> This is used to set your name globally in Git, which will be associated with the commits you make.

13. git config --global user.email "Your email"
	-> This is used to set your email address globally in Git, which will be associated with the commits you make.

14. git config --list
	-> For seeing the current global configurations in git.

15. git config --global core.editor "code --wait"
	-> for setting the code editor as visual studio code and wait indicates that it waits for the editor to close the current opened files in the editor.

16. git commit
	-> this will open the COMMITMSG file in which we have to enter the commit message and when we close that file it will automatic commit will happen.

17. git diff hash_value
	-> for checking the changes between particular commits. that hash_value is used for uniquely identify between different commits.

GIT Bash Indicators :-

jills (master #) GitGithubMasterclass 
	- here master indicates current branch and # means it has some changes that are not yet inside repository.

jills (master +) GitGithubMasterclass
	- here + indicates that the changes are staged.

jills (master) GitGithubMasterclass
	- it means that no changes that are to be added.

jills (master *) GitGithubMasterclass
	- this means that item is already in git repository that now has new version.
