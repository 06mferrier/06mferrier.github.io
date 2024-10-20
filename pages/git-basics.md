#Getting Started with Git

Git is an industry standard tool for version control and collaboration. Being comfortable with the basics is essential. A high level summary of the process of working with Git is below:

* Clone the repository,
* Create a new branch,
* Make changes to your new branch,
* Commit and push your changes,
* Make a pull request to have your changes merged with the main branch.

To the uninitiated, the terminology used above will be unfamilar. The following table will shed some light on these terms.

|Git cheat sheat|
|Term|Meaning|
|---|---|
|Repository| |
|Branch| |
|Commit| | 
|Push| |
|Pull| |

##Basic Git Workflow

The steps below will walk you through how to clone a repository, create a new branch, commit and push your changes, and make a pull request.

⦁	Get started
Open windows command prompt.
⦁	Clone the repository
If this is your first time contributing, you will need to clone the remote repository. Use command “git clone <repository-url>”, replacing <repository-url> with the URL of the repository you wish to clone.
⦁	Set directory
Set the current directory to your local repository.
⦁	Have you contributed before?
If you have contributed before, switch to the main branch with command “git checkout main”, and use “git pull” to ensure that your local repository is up to date.
⦁	Create new branch
Use command “git branch <branch-name>” to create the new branch for your changes, replacing <branch-name> with your chosen name for the new branch.
⦁	Switch to new branch
Switch to the new branch using command “git checkout <branch-name>”.
⦁	Make changes
Make changes as per DevOps ticket
⦁	Commit changes
Use command “git add .” to stage all new or modified files. Commit your changes with “git commit –m"<comment>””, replacing <comment> with a meaningful comment about your changes.
⦁	Push your branch
Use command “git push –set-upstream origin <branch-name>” to push your branch to github.
⦁	Create a pull request
Open the github URL of the remote repository. Your new branch should be visible. Navigate to your branch and press the “Compare & pull request” button towards the top of the page. Add a title and description as appropriate, and press the “Create pull request” button.

If there are no conflicts, it will be possible to review the pull request and merge the new branch with the main branch. If there are conflicts, then it could be that two people have made changes to the same line of a file, or one person has edited a file, and another person has deleted it. If there are conflicts present, github will make it obvious that this is the case.
Consider the scenario where the repository contains a file named data.txt. You edit the first line of data.txt as part of the changes you are making to your branch. Meanwhile, someone else makes changes to the first line of data.txt in their branch, submits their pull request and has it merged with the main branch before you finish your changes. When you make the pull request for your changes, github will flag up that there are conflicts that must be resolved. You can still make the pull request, and resolve the conflicts afterwards.
Conflicts arising from competing changes can be resolved on github. When viewing a pull request with conflicts, there is a “resolve conflicts” button. Clicking this button will bring up an editor, comparing the two changes. There are markers <<<<<<, >>>>>>, and ====== separating the two changes. Resolve the conflict as appropriate, making sure the markers are deleted (including the branch names), and press the “mark as resolved” button. If there are other conflicts to resolve, use the next/previous buttons to navigate through them until they are all resolved.

