# Git Cheat Sheet

A cheat sheet for Git commands.

#

create and delete branches https://github.com/Kunena/Kunena-Forum/wiki/Create-a-new-branch-with-git-and-manage-branches
.gitignore File – How to Ignore Files and Folders in Git https://www.freecodecamp.org/news/gitignore-file-how-to-ignore-files-and-folders-in-git/#introduction

1. create a .gitignore file
   touch .gitignore
2. Add the Paths and files
3. Push your changes

Remove from remote repository

1. Add to .gitignore
2. Remove from Git Tracking
   git rm -r --cached path_to_your_folder/

get username and email
git config user.name
git config user.email
set username and email
Local (go to the repository directory)
git config user.email example@email.com
git config user.name "example"
global
git config --global user.email example@email.com
git config --global user.name "example"
Adding locally hosted code to GitHub https://docs.github.com/en/migrations/importing-source-code/using-the-command-line-to-import-source-code/adding-locally-hosted-code-to-github

1. Initialize the local directory as a Git repository
   git init -b BRANCH-NAME
2. Add the files in your new local repository
   git add .
3. Commit
   git commit -m "First commit"
4. Ddd the URL for the remote repository
   git remote add origin REMOTE-URL
5. Verify that you set the remote URL correctly
   git remote -v
6. Push
   git push origin BRANCH-NAME
7. Set the remote as upstream branch
   git push --set-upstream origin BRANCH-NAME

Push existing repository to new remote

1. Create new branch if needed
   git checkout -b BRANCH-NAME
2. Rename origin upstream
   git remote rename origin upstream

3.Add New repository URL
git remote add origin REMOTE-URL 4. Push to the desigered branch
git push origin BRANCH-NAME 7. Set the remote as upstream branch
git push --set-upstream origin BRANCH-NAME
Remove file history from header
git filter-branch --index-filter 'git rm -r --cached --ignore-unmatch <DIR/FILE>' HEAD
Deploy React app to Github pages https://www.freecodecamp.org/news/deploy-a-react-app-to-github-pages/

1. Add locally hosted code to GitHub (see above)
2. install gh-pages packages
   npm install gh-pages --save-dev https://www.npmjs.com/package/gh-pages
3. Add keys to script inside package.json
   "predeploy": "npm run build",
   "deploy": "gh-pages -d build",
4. Add homepage field to top of package.json
   "homepage": "URL",
5. Deploy
   npm run deploy
