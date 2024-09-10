# task1

01 Git configuration
git config --global 
user.name “Your Name” Set the name that will be attached to your commits and tags.
git config --global 
user.email “you@example.
com”
Set the e-mail address that will be attached to your commits 
and tags.
git config --global 
color.ui auto Enable some colorization of Git output.
02 Starting a project
git init [project name]
Create a new local repository in the current directory. If 
[project name] is provided, Git will create a new directory 
named [project name] and will initialize a repository inside it.
git clone <project url> Downloads a project with the entire history from the remote 
repository.
git rm [file] Remove file from working directory and staging area.
04 Storing your work
git stash Put current changes in your working directory into stash for 
later use.
git stash pop Apply stored stash content into working directory, and clear 
stash.
git stash drop Delete a specific stash from all your previous stashes.
05 Git branching model
git branch [-a] List all local branches in repository. With -a: show all branches 
(with remote).
git branch [branch_name] Create new branch, referencing the current HEAD.
git rebase [branch_name]
Apply commits of the current working branch and apply them 
to the HEAD of [branch] to make the history of your branch 
more linear.
git checkout [-b]
[branch_name]
Switch working directory to the specified branch. With -b: Git 
will create the specified branch if it does not exist.
git merge [branch_name] Join specified [branch_name] branch into your current branch 
(the one you are on currently).
git branch -d [branch_
name]
Remove selected branch, if it is already merged into any other. 
-D instead of -d forces deletion.
03 Day-to-day work
git status
Displays the status of your working directory. Options include 
new, staged, and modified files. It will retrieve branch name, 
current commit identifier, and changes pending commit.
git add [file]
Add a file to the staging area. Use. in place of the full file path 
to add all changed files from the current directory down into 
the directory tree.
git diff [file] Show changes between working directory and staging area.
git diff --staged [file] Shows any changes between the staging area and the 
repository.
git checkout -- [file] Discard changes in working directory. This operation is 
unrecoverable.
git reset path... Revert some paths in the index (or the whole index) to their 
state in HEAD.
git commit Create a new commit from changes added to the staging area.