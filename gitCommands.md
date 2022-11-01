# Some common git commands and procedures with MAC in Terminal. Node heavy.

## TO SETUP REPOSITORY WITH GIT. (ONE TIME ONLY PER FOLDER).

1.  ENSURE FOLDER LOCATION in MAC terminal or VS terminal.

        - command line: ls //shows folders/files in "cd": current directory
        - cd filename //Changes Directory to filename

2.  initilize to connect with Git Hub

    git init

3.  change name from master to main

    git branch -m main

4.  add of all files in folder && commit -m "message of work done for update"

    git add . && git commit -m "message here"

5.  GO TO YOUR GIT HUB REPO SECTION AND CLICK ADD NEW.

    - If Open Source Practice, Simply specify a unique name for the repostion and CREATE it.
    - COPY the Code Block to "Push New Repository from Local Device"
    - Go back to Terminal or VS terminal
    - PASTE in Command Line and ENTER

6.  Your New Repo should be visible on Git Hub.
    - Simply Refresh (Command R) your Git Hub webpage you Copied your last command from.
    - (ONE TIME ONLY PER FOLDER).
7.  IN CORRECT FOLDER update any additions or Mods to the Repo that was made.

    git add . && git commit -m "message" && git push

#### Pull files added on git to add localy on VS Code

       git pull

#### update an repo connected with git already

       git add . && git commit -m "message" && git push

### tells what you can push or fetch

       git remote -v

### get latest updates

       git fetch

### Latest version of code

       git pull

### current status

       git status

### shows branches. (command q to quit)

       git branch

### make a copy of main branch... -b will see if specified branch exists, if not, it will create it.

       git checkout -b new-branch-here

### from **_.. git main...._**... merge changes of branch

       git merge new-branch-name

### delete a branch

       git branch -d new-branch-here

### Make a PR..(Pull request)

       git push branch-name

### Get rid of changes made

       git stash

### Git doesn't exist...Probably X-Code on Mac. Either Update in Terminal or in App

       xcode-select —install
