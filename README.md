//Updating Config list
git config --list
git config --global user.name “[name]” 
git config --global user.email “[email address]”
// View total no. of branches 
git branch
// to create a develop branch 
git branch develop
//Checkout branch or switching to a branch or //moving to any new branch.
git checkout develop 
/Adding new files:
touch filename
//How to make changes using vi
vi filename
press i
type ur lines of code
press escape key
press :wq
enter key
//To see the status of the tracked files in staging area
git status
//git add command will add any modifications of source code or any new additions to staging area. 
git add filename
git add . 
//To untrack the modifications done and added to staging you can use restore or reset. i.e to revert back.
git restore --staged testfile.txt
git add .
git commit -m “comments”
git log
git reset --hard commitID
//To see logs for the commits done so far.
git log
git show commitID
//Will show modifications done in source code 
Git diff
git diff --staged
//Will pull the modifications done by anyone in same project to your local
Git pull
//Merging changes and pushing to remote
git merge branchname
git push
//Stash command helps you to save or park your changes for temporary purpose and continue making further 
changes, whenever we are ready we can bring back the saved/parked changes and do the commit and push to 
remote repository. It follows LIFO.
git stash save
git stash list
git stash drop
git stash pop
git stash list
git stash pop stash@{1}
git stash pop stash@{0}
//Use tags for your multiple releases
git tag -a <tag-name> -m "tagging message" (creates an annotated tag)
git push origin tagname
git tag
git show tagname
git revert 
//rm - Remove file from git project repository, clean – Remove untracked files or directory from your git 
//repository
git rm filename
git clean -n
git clean -fd
