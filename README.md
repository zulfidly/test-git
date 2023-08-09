# commit & push : branch3

### initialise a git
- ```git init```
- ```git branch -M main```, this will make 'main' as default branch


### open Terminal within active folder in VS Code
- create the folder
git init
git remote add origin https://github.com/zulfidly/airbnb-clone.git
git pull origin main

### ```git branch -M branch``` can also be used to switch branches
### 

### ```git clone 'link'```
- create a folder where we want to place this repo in
- git clone includes the remote link automatically, so it's more straight forward

### git init
git add ./index.html ./projects.html ./contact.html ./about.html
git add ./main.js ./homeMobile.js
git add ./asset/
git commit -m "description"
git remote add origin 'link'
git push -u origin main

### note:
- any edits made in a branch, can only be pushed into the active branch where the work is being done
- every additional branch will create a pull request on GitHub as "Compare & pull request"