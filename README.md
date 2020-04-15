### Auto link local branch to remote (even not existent)
git config --global push.default current

### Git pull all folders from parent
find . -mindepth 1 -maxdepth 1 -type d -print -exec git -C {} pull \;

### Create branch, commit & push
git  checkout -b feature/dl-456-modal-height
git add *scss
git commit -m "DL-456 modal height" --no-verify (if Angular runs checks)
git push -u --no-verify (if Angular runs checks)
