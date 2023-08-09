### initialise a git
- ```git init```
- ```git branch -M <default_branch>```, this will make 'main' as default branch
- ```git commit -m 'msg'```
- ```git remote add origin 'link'```
- ```git push -u origin <branch_name>```

### Create a new branch
- ```git branch -M <branch_name>```

### Switching branch properly
- do this before making any edits, git will remember what edits made in which branch and link them together
- ```git checkout <branch_name>```, preferably without any pending commits

### Delete a branch locally
- to check: ```git branch -a```
- 


### Clone a repo
- create a folder where we want to place this repo in
- ```git clone 'link'``` includes the remote link automatically, so it's more straight forward 
(compared to ```git init``` + ```git add remote origin``` + ```git pull```)

### note:
- to create an update, 
- any edits made in a branch, can only be pushed into the active branch which the work is being done
- every additional branch will create a pull request on GitHub as "Compare & pull request"
    - or, we can see the "Open pull request" button
- click "Open pull request"
- click "Create pull request"
- click "Merge pull request" --> "Confirm merge"
- message: "Pull request successfully merged and closed". At this point, "Delete branch" button is visible
- branch "main" is now updated