## This example assumes ```<default_branch>``` as ```main```

### Initialising git
- ```git init```
- ```git branch -M <default_branch>```, this will make 'main' as default branch
- ```git remote add origin 'github_link'```

### Commit & push to a git
- ```git commit -m 'msg'```  
- ```git push -u origin <current-work-branch>```

### Create a new branch
- ```git branch -M <name-of-new-branch>``` 
    - this will create a branch locally first
    - remote repo will get updated once pushed

### Switching branch properly
- do this before making any edits, git will remember what edits made in which branch and link them together
- ```git checkout <branch_name>```, preferably without any pending commits

### Delete a branch
- note: local branch and remote branch may not be the same
- checkout to default branch first: ```git checkout <default_branch>```
- check local git branches : ```git branch -a```
- delete a local branch: ```git branch --delete <branch_name>```
- delete a remote branch: ```git push origin --delete <branch_name>```

### Synchronising branch list 
- ```git fetch -p```
- this will update local following remote branches

### Clone a repo
- create a folder where we want to place this repo in
- ```git clone 'link'``` includes the remote link automatically, so it's more straight forward 
(compared to ```git init``` + ```git add remote origin``` + ```git pull```)

### note:
- to create an update, 
- any edits made in a branch, can only be pushed into the active branch which the work is being done
- every additional branch will create a pull request on GitHub as ```Compare & pull request```
    - or, we can see the ```Open pull request``` button
- click ```Open pull request```
- click ```Create pull request```
- click ```Merge pull request``` --> ```Confirm merge```
- message: ```Pull request successfully merged and closed```. At this point, ```Delete branch``` button is visible
- branch "main" is now updated