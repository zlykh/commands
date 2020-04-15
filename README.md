### Auto link local branch to remote (even not existent)  
git config --global push.default current  

### Autostash on pull
git config pull.rebase true  
git config rebase.autoStash true  

### Git pull all folders from parent
find . -mindepth 1 -maxdepth 1 -type d -print -exec git -C {} pull \;  

### Create branch, commit & push  
git  checkout -b feature/modal-height  
git add *scss  
git commit -m "modal height" && git push -u  
(if Angular runs checks) git commit -m "modal height" --no-verify && git push -u --no-verify   

### Push overwrite
git commit --amend --no-edit && git push -u --force  
git add * && commit --amend --no-edit && git push -u --force  

### Pull master
git checkout master && git pull
