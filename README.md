# git
basics of git
### Git is a distributed version control system-
In git every body has a local repository. Your local repository has all the information that your remote repository has based on the last time when you synced them together.So the good thing about this is that if you don't have access to that remote repository then you can still view the changes. So in a way every developer has the entire backup of the repository.
‌
So in worst case scenario any thing happening to remote repository every developer has a copy of that same repository on there machine.

### One time changes-
#### step1
-Install git
#### step2
-check if git is successfully installed-
#### git --version
#### step 3
set global config variables.
#### git config --global user.name "Vaibhav Poonia"
#### git config --global user.mail "pooniavaibhav@gmail.com"
to check the set values-
#### git config --list
use following command to get the help
#### git help verb (replace verb with the command whos einfo you want)
#### git help config
### Cases
You can have two cases -
#### case1
you have a existing project on your local machine that you want to track using git.
#### case2
you already have a project running remotely.

## Case 1
navigate to your directory where your code is presnt and run-
### git init
your directory will create a .git file that contains all the info abt your code. now run git status command to chack the status of your git code.
### git status
### git ignore file
It is a simple text file that contains the file that we want git to ignore.just enter the files you want to ignore.
### nano .gitignore
here write the file name you want tocheck and run git status command you will see that file mentioned in git ignore is removed from list of file.
## While working with git there are three stages we should know about.
### WORKING DIRECTORY
### STAGING AREA 
### GIT REPOSITORY
#### JOURNEY
Untracked and modified files will be in our working directory.When we run git status command so we get a lsit of those files.Staging area is where we organise what we want to be committed to our repository.The reason for the staging area is so we can pick and choose what we want committed. So if we have made changes in lot of files we can stage those files and commit them at once.
### Adding files to staging area-
use folllowing command to add to the staging area-
#### git add -A
This will add all the files to the staging area.now check using git status command to see files ready to commit.
### remove files from staging area
use following command to remove file from staging area.
#### git reset
or you can give a file name-
#### git reset file.py
## Commit code
### git commit -m "Initial commit"
-m adds the message to the commit which is very important.
### git log
git log gives the info about your commit.
## CASE 2
we want to track existing remote project with git.
### Step1
clone the repository from the remote repo-
#### git clone url where to clone
#### git clone ../remote_repo.git .
### Viewing information about the remote info
#### git remote -v
gives info about fetch and push
#### git branch -a
gives info about branches.
## Pusing changes
## Step1
### git diff
it shows the changes you have made.
## Step2
check your status using git status.
## Step3
add files in staging area using git add command
## Step4
commit files using git commit command.
## Step5
as we are making changes there is a possibility that some other has also made chnges in code so use following command.
### git pull origin master
here origin is the name of our remote repo and master is the branch we want to push.


