git init
git status

git add .
git add filename1 filename2
git commit -m "first commit"
git log

git config --global user.email ""
git config --global user.name ""

git checkout e639a19387999d47ff2637e3939abb7a8e7094ed
git checkout master

// for branches
git branch
git branch second-branch
git checkout -b third-branch

git merge third-branch

git switch third-branch // same as git checkout third-branch
git switch -c fourth-branch // same as git checkout -b fourth-branch


git ls-files
git rm test.txt

//to revert changes
git checkout init.txt
git checkout .  // revert all to head
git restore init.txt
git restore .  // revert all to head

// to delete untracked file
git clean -dn //for checking
git clean -df // force to delete

// undo staged changes
git restore --staged init.txt // latest
git reset --> git checkout xxx // old way

// to delete latest Head to go back one step
git reset --soft HEAD~1    // soft reset, only commit
git reset HEAD~1 // file will be delete from staging area
git reset --hard HEAD~1 // remove commit, remove changes, remove file, remove from stage area

// delete branches
git branch -D fourth-branch

// stash
git stash apply
git stash
git stash list
git stash push -m "third feature"
git stash drop 0/ git stash clear


git merge --squash feature // only one commit need
git merge --no-ff // no fastforward merge

git merge --abort // exit the merge. rollback
git log --merge
git diff // check different
git cherry-pick <id> // only merge specify commit


//tag
git tag 1.0 <id>
git tag // to list
git show 1.0 // to display tag detail