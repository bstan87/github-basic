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