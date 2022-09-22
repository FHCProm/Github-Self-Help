# Github-Self-Help
This is a self-help guide for forgetful people like me 
## Resource is taken from videos below:
`````
1. https://www.youtube.com/watch?v=RGOj5yH7evk&t=1514s

`````
## Basic Git commands:
````
1.git clone
2.git add .
3.git commit -m "message"
4.git push
5. git status

````
## Connect your local machine to GIT using SSH. 
````
Reason to use SSH:remove the need of personal access token that needs to be entered everytime commit is done. 
In your terminal:
Step 1: ssh-keygen -t ed25519 -C "your_email@example.com" (save in ~/.ssh file)
Step 2: open up git bash(wont work in windows terminal) , then    eval "$(ssh-agent -s)"
Step 3: ssh-add ~/.ssh/"your private key file name"

In Github Setting page:
Step 1: Copy the "your public key file".pub (pub stands for public key)
Step 2: paste into your github "new SSH key"

For testing SSH connection:
Step 1: ssh -T git@github.com

For pushing local repo to Github for the first time :
Step 1: git remote add origin "git@github.com:profile-name/repo-name.git
Step 2 : git push
````


## Git Workflow
````
I hope i learn this earlier but it still requires tacit understanding among teammates. 
Useful commands for mixing magics：
1. git branch 
2. git checkout "your branch"         ---> go to that branch
3. git checkout -b "your branch"      --->create new branch
4. git diff "a branch"
5. git merge "a branch"
6. git branch -d "a branch"           --->delete a branch
7. git merge MASTER/MAIN              --->bring in changes from local main branch into the branch that your are working so that you can solve conflict from time to time . To prevent nuclear bomb fusion later.
8. git pull       (for master/main)   ---> do it often whenever someone make changes to the main branch in GITHUB. So that you can `git merge Master` to prevent nuclear fusion later.
````


## Technique that may help u to clear commits flood
````
1. git reset "HEAD"                   ---> It does not remove the changes that you have made. 
````






