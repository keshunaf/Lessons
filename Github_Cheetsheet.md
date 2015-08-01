# Github CheatSheet

Be mindful, you must write your commands very specificly. The Terminal is an area of great power and with great power comes great responsibility (aka. You can do a lot of cool stuff here, you can also mess up your computer here). Capitols and Spacing is very important. Do not type in a command unless you know what it does.

### Warnings!!!
- -f (an "f" flag, forces an action that may not be safe)
- sudo (sudo, circumvents safety checks by running command as a superuser)
- master (this is dealing with the master branch, your main copy or more specificaly EVERYBODY's MAIN COPY)

#### Notes
- text within `<>` must be specific to you.
- branch names must not have spaces use CamelCase or snake_case
  - CamelCase (capitols at the begining of words with no spaces)
  - snake_case (lowercase with underscores)

----------------------------------------------------------------------------------

## Our Process In This Class

#### 1 - Find your folder
Traverse your Terminal (or Command Prompt for windows) using the following commands

For Mac
  - ls 
  - cd `<folder_name>`

For Windows
  - dir
  - - cd `<folder_name>`

#### 2 - Clone
- `git clone <http_repo_address>`
- `cd <folder_name>`

#### 3 - Check your git
- `git status`
  - note which branch you are on
  - note what changes have staged or have not been staged

#### 4 - Branch (if needed)

For this class use your github username(s) for your `<branch_name>` (example: individual branch_name: JoCoding / team branch_name: JoCoding-SueMastery)

- `git checkout -b <branch_name>`

#### 5 - Stage
- `git add .`
- `git status`
- `git commit -m "<commit_message>"`

#### 6 - Push
- `git push origin <branch_name>` - NEVER PUSH TO MASTER!!!!!!!

I'll say it again, NEVER PUSH TO MASTER

----------------------------------------------------------------------------------

### Commands that you may use

#### Commands
```
- ls - to list available files and folders, it is dir for windows
- cd <folder_name> - change directory to foldername
- git branch - to check for current branch and list of available branchs
- git branch <branch_name> - makes a new branch using <branch_name>
- git checkout <branch_name> - to switch branch named <branch_name>
- git checkout -b <branch_name> - creates and switches to branch named <branch_name>
- git branch -d <branch_name> - deletes branch named <branch_name>
- git add <file_name> - add a file to staged
- git add . - add all files
- git add -u - updates if you deleted a file
- git commit -m <commit_message> - commits your changes and labels your commit so it can be looked up later, if you don't type the "m" flag you'll be stuck, ask an intsructor for help
- git pull origin <branch_name> - pull current <branch_name> on to your current branch
- git pull --rebase origin <branch_name> - add code from <branch_name> and add it to your current branch local to resolve conflicts before pushing to github
- git push origin <branch_name> - pushes branch, NEVER TO MASTER
```


### later addition - pull someone else's work

if you want to pull someone else's work follow these steps
- clone the repo as you would normally
- if you have done work, you need to push it to github or stash it
  - `git stash` - this is going to be saved but it is difficult to retrieve
- you need your partner's branch on your computer, check with
  - `git branch`
  - if you do not see your parnter's branch type
  - `git branch <branch_name>`
- now switch to their branch
  - `git checkout <branch_name>`
- and pull their work
  - `git pull origin <branch_name>`
- go to your files and they will have your partner/team's work
