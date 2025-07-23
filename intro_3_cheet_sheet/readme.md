/*
adding intire folder to github:

first of all create a git repository
then open the folder with git bash (using right click) which we want to upload
// a git bash terminal gets opened

git init
git add .
git commit -m <- description ->
git branch -M main
git remote add origin <- repository name ->   
// specify the repository made at step one for uploading 
git push -u origin main

//if error arrises ! [rejected]        main -> main (fetch first)
//error: failed to push some refs to 'https://github.com/mihirgupta665/temporary.git'
then add below commands as project need to be pushed through a new branch

git branch -b <- new branch name ->
git add .
git commit -m "message"
git push -u origin <- new branch name ->

*/

/*
Git hacks:
 git.io  -> takes a input as a git link and shortens it
 lines could be selected by shift key adn could be send by copying the link
 blame: is used to tell who has worked on a specified stuff and tell or what was added(green) or removed(red)
*/