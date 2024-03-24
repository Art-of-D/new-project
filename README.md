Jira Ticket:

Task Title: Set up new Git repository and create development branch for 'new-project'

Task Description:

As a developer, I need a new GitHub repository for 'new-project' and i need a development branch so that I can work on new features without affecting the main branch. 
Readme file should contain step-by-step instructions on how we can do it ourselves.

Expected Results:

A new branch called "development" is created and the user is able to switch to it successfully.
A new file called "README.md" is created and step-by-step instructions is added to it successfully.
The changes to the "development" branch are committed with a commit message successfully.
The changes from the "development" branch are merged into the "main" branch successfully.

Instruction:
Create a new repository on GitHub
Go to dir where you want to manage files by ~ cd ./FILE_NAME
Then create dir by ~ mkdir new-project
After init the new repository ~ git init
Create relation between local and remote repository:
~ git remote add origin URL_OF_REMOTE_REPO
~ git branch -M main
Create the new file by ~ touch readme.md
Add some text ~ nano readme.md
Save changes and commit it by commands:
~ git add . (For only selected file use ~ git add FILE_NAME.TYPE)
~ git commit -m "init"
(If you need you can check status by  ~ git status )
Push it to remote repo by ~ git push -u origin main
To create new branch use ~ git switch -c "NAME"
Add some changes to your file ~ nano readme.md
Save them and commit:
~ git add .
~ git commit -m "NAME"
~ git push -u origin BRANCH_NAME
Merge it with the main branch:
~ git switch main
~ git merge BRANCH_NAME 
Commit after merge git commit -m "NAME"
Check the status by ~ git status
Push it to remote repo by ~ git push

Definition of Done (DoD):

Link to new-project Readme file