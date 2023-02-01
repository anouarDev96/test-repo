# git config -- list

==> to list git configuration

# :q

==> to quit

# git config --global

==> to update or create user crendentials.

# git init

==> to initialize git repository

# git status

==> to check the current status of the repository meaning ( files added or deleted or updated would be diplayed)

# .gitignore

==> is a file that prevent certain files or directories from being added to the source code

# git add . | filename.ext ...

===> it is used to add files to staging area

# git reset .

===> is used to remove the files that have been added to the staging area

# git log

===> it is used to log the commits

# shortcut : git commit -a -m "<messsage here>"

===> this command add the files to the staging area and commit them

# git remote

===> check if your local repository is linked with any remote repository

# git remote add origin https://github.com/anouarDev96/test-repo.git

===> origin is the name of the remote repository and url (its location)

# git remote -v || git remote show origin

===> show information about remote repository

# git push origin master -u

# -u ::===> allow us to use cammand "<git pull>" without any additional arguments

===> push the changes to the remote repository

# git fetch

===> fetches all latest changes fron the remote repository

# git merge origin/master

===> marges between local repository master and remote repository master

# git pull (and without -u flag) origin master

===> combination of( fetch + merge) with one command

# git clone

===> allow to clone remote repository

# git branch

===> list all the branches

# git branch - M <name of the branch>

===> to rename a specific branch

# git branch <name of the branch>

===> to create a new branch

# git branch -d <name of the branch> (d -> softdelete, D -> hard (forced) delete)

===> delete a specific branch

# git checkout <name of the branch>

===> switch to the targeted branch

# git checkout -b <name of the branch>

===> create and switch to that branch

# git checkout -

===> to switch to most recent branch that you've switched from

# what is merge conflict ?

===>
trying to merge two branches that modify the same lines of code

# how to resolve merge conflict?

===> 1/ which files are afected 2/ choose the correct code 3/ commit 4/ or go back to the state before the merge

# git merge --abort

# git diff

===> to see defferences between two commits

# what is a Fork ?

===> 1/ copy the repo into your own account 2/ it also keeps link to the original repo 3/ the original is named "UPSTREAM" repository 4/ work on a feature then send pull request to merge that code to the original from the fork 5/ the author of the original repo can review your change and the decide if he should merge or not

# how to fork ?

===> 1/ pick a repository 2/ click on fork 3/ clone the project locally 4/ switch the branch 5/ add a feature 6/ stage the changes 7/ commit the changes 8/ git push origin <name of the branch> 6/ wait for the review by the author

# git reset

===> if you staged files you can undo it by running this command

# git reset 512ce3595e2541c4399a5c649eae05ce73fe96a6

===> if you pushed a bad commit and you wish to revert back to the previous commit and HEAD will move to the commit

# git reset --hard 512ce3595e2541c4399a5c649eae05ce73fe96a6

===> one difference is it delete all the files for that bad commit

# you should never reset code on github !!! (commits that have been pushed to the remote repository)

# git revert 512ce3595e2541c4399a5c649eae05ce73fe96a6

==> the only defference between revert and reset is that commit is still in the commit history

# git commit --amend -m < insert message here>

==> it is used to update last commit bad message

# git commit --amend --no-edit

==> move the file to the staging area with the same message

# git stash

===> move the code that is not ready

# git stash save <name of the stash>

===> save the stash with a name

# git stash list

===> to list all the stashes

# git stash pop

===> to remove the last stash

#git stash apply <index>(retreived from git stash list)

# what is rebase ?

===> take feature branch and rewrite history that will be making it look like that you started working on feature branch with latest update from the master branch or keeps the feature branch in sync with the master branch

# git rebase master

===> create extra branch from your feature and do rebase on that branch
then make sure that everyting is okay (delete that temporary branch) if it is do it on the feature branch

# git rebase master --interactive

===> replace pick with squash it will pick commits message from all of them and combine them into one single message with that original commit
