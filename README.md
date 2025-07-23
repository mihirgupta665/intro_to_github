# intro_to_github
This is my first Git Repository

changes are made final by  commit its like take the creenshot and save it to the memory thus saving the history  
-- version  :  to test the version
ls : to see the directories
clear : to clear the directories
pwd : prints the current working directory

/*
Configuring GitBash:

git config --global user.name="_name_"                // seting the username same as of git hub  by globally means always sets the changes in this github account only
git config --global user.email="github_gmail"         // setting the githubgmail
git config --list                                     // list down the content of git config
*/

git clone "_link_" : is used to clone a git repository to our local system
ls : shows files in a directory but       ls -Force : shows all hidden files of a directory(including .git -> which are present in each folder of  which gits saves the history or runs)
Note: in git hub we dont need to add(staged) the changes we could directly commit them but in git we need to first add the changes(staged : ready to be saved) then commit(save) them. 
git status:  gives the status of files whether they are up to date or not
git branch:  to get the name of your git branch
git pull origin main: these is used to pull the changes made in the file of github 

/*
    git status:

    untracked: new files which git has not yet tracked
    modified: changed
    staged: file is ready to be committed
    unmodified: unchanged
*/

git add <- file name -> adds new or changed files of our current working directory to git staging area.
git add . : is used to add all the modified content alltogether.
git restore --staged <- file name  -> : to unstage a file
commit: is a record of change       // after commit the chnages will be saved but not published to publish we need to pust the changes.
git push origin main : upload local repo content to remote repo content
//origin is the name of the default repository in which changes will be displayed
//main is the branch in which we are pushing the changes


As above stated pull repository could be executed only if repository is first made in the github and then its been cloned and pulled(if changes made at github)
But as we traditionally makes folders first then project so here comes the role of init commands which initializes the repository

So to make folder first and then creating its git repository goes the following :

create the folder , change your directory to the very same folder then write git init
git init: 



