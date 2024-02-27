# Git/Github

Git is a free and open source distributed version control system

To check git version on your machine, opem cmd and enter ->   git -v

to check the username and email configured for git -> git  config --global user.name  /  git config --global  user.email

Basic terminologies -

repository/driectory/folder
init/initialization - starting git for our folder
untracked area/untracked files
staging area
commits
local repo
remote repo
push

There are basically three areas in git - untracked area, staging area and commit area.

staging area is just pre-comit area, to track files we need to first stage them and then to save them we need to commit those changes.
Commiting is basically saving a version of our project, a checkpoint/milestone being saved. 

First select the folder/repository where we want to initialize 'git'

Open that directory in any CLI or git bash and enter - git init

![image](https://github.com/Sanketsingh77/vette/assets/35081012/34f1790f-6b6e-4de7-ac2d-48469f84046b)

to check current status of our repository - git status (gives a status overview of our directory)

Now to any changes made to our repo , we need to move it to the staging area - git add filename

![image](https://github.com/Sanketsingh77/vette/assets/35081012/14a699db-50a5-4831-b5a4-e5494a470585)

To move multiple files to staging area - git add filename1, filename2, filename3

To add all the untracked files to the staging area - git add .

To add all the files in the staging area to commit area - git commit -m "your message"

This will save one version of our code.

![image](https://github.com/Sanketsingh77/vette/assets/35081012/f1223e56-cc80-4451-b8a0-e55911466c52)

To check all the history of versions of our code - git log


![image](https://github.com/Sanketsingh77/vette/assets/35081012/fafb9de4-e321-4263-93fd-15e6282f927b)

we can see there's only one log here

Supoose we have 100 files and want to stage only 90 files and ignore 10 files. For that we have to separately write the names of the 90 files
which can be very troublesome so we use something as '.gitignore' file and this file will make sure that all the names of files written in this
file will be ignored and not be moved to the staging area, they will remain untracked.


Now that we have created a git repository and pushed all of our changes, it's still present in our local repo in our local system. We have to 
move it to remote repo so that we can access it from anywhere and collaborate with people , etc. We use GitHub which is a web based hosting 
service for our git repositories.

We create a new repo in github thorugh the UI and then upload our files/folders to GitHub either though the UI or CLI.

To check if any remote repo is already present - git remote -v

If not present, then we add a remote repo - git remote add origin githubRepo-https-link

To switch to main branch - git branch -M main

To push our commits to the branch - git push origin branch-name








