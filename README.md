# flutter-video-tutorial-link-one
Flutter video tutorial link one

[Flutter video tutorial link one](https://rzrasel.github.io/flutter-video-tutorial-link-one)

### GIT Command
```git_command
git init
git remote add origin https://github.com/rzrasel/flutter-video-tutorial-link-one.git
git remote -v
git fetch && git checkout master
git add .
git commit -m "Add Readme & Git Commit File"
git pull
git push --all
```

### Reducing the repository size using Git
```
Navigate to your repository:
cd my_repository/

Change to the branch you want to remove the big file from:
git checkout master

Use filter-branch to remove the big file:
git filter-branch --force --tree-filter 'rm -f path/to/big_file.mpg' HEAD

Instruct Git to purge the unwanted data:
git reflog expire --expire=now --all && git gc --prune=now --aggressive

Lastly, force push to the repository:
git push --force origin master

Your repository should now be below the size limit.

-- git filter-repo --to-subdirectory-filter "$REPO_NAME"
-- git reset --hard
-- git reflog expire --expire=now --all
-- git gc --prune=now
```

Navigate to your repository:
```
cd my_repository/
git checkout master
git filter-branch --force --tree-filter 'rm -f path/to/big_file.mpg' HEAD
git reflog expire --expire=now --all && git gc --prune=now --aggressive
git push --force origin Flutter-Tutorial-Navigate-To-Another-Screen-One
```