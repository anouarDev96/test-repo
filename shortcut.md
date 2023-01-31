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
