### Auto link local branch to remote (even not existent)  
git config --global push.default current  

### Git pull all folders from parent
find . -mindepth 1 -maxdepth 1 -type d -print -exec git -C {} pull \;  

### Create branch, commit & push  
git  checkout -b feature/modal-height  
git add *scss  
git commit -m "modal height" --no-verify (if Angular runs checks)  
git push -u --no-verify (if Angular runs checks)  

### Pull master
git checkout master && git pull
