PS C:\Users\CasmerAntonSiega\Siega_Practical> ( # "project name that all folder that you make and save." then here's the step sir)
PS C:\Users\CasmerAntonSiega\Siega_Practical> git init
echo "# Project Name" > README.md
echo "print('Hello World')" > sample_code.json
echo "__jsoncache__/\n*.log\n*.tmp" > .gitignore
git add .
git commit -m "Initial commit: add README.md, sample_code.json, and .gitignore"
(I Create a GitHub repository)
git remote add origin https://github.com/Casiega/Casmer-Anton-B.-Siega.git
git branch -M main
git push -u origin main
git checkout -b feature-UI
( # then if new branch switched in feature-UI next is I make a sample of html)
 echo "<!DOCTYPE html><html><head><title>UI</title></head><body><h1>Hello from CasmerGwapo</h1></body></html>"ui.html
 git add ui.html
 git commit -m "Add basic UI template in ui.html"
 git checkout -b feature-Backend
 echo "\ndef add(you, me): return you + me" >> sample_code.json
 git add sample_code.json
 git commit -m "Add backend logic for addition function"
 git checkout main
 ( # Next steps Merging the featured-UI)
 git merge feature-UI
 git merge feature-Backend
( # Resolve the conflicts manually in your editor )
git add .
git commit -m "Resolve merge conflicts and complete merge"
( # Create a version tag and simulate a release)
git tag v1.0
git push origin v1.0
( # Simulate error correction and cherry-picking)
git checkout feature-Backend
echo "raise Exception('Simulated backend error')" >> sample_code.json
git add sample_code.json
git commit -m "Introduce simulated error in backend code"
(# REMOVING the error commit using Git history modification (Interactive Rebase))
git log --oneline
git rebase -i HEAD~2
pick abc123 Introduce simulated error in backend code, pick def456 Add backend logic for addition function
drop abc123 Introduce simulated error in backend code, pick def456 Add backend logic for addition function
(# Cherry-pick a commit from feature-UI to main)
git checkout main
git log feature-UI --oneline
git cherry-pick <commit-hash>
(# Push the changes to the remote repository)
git push origin main


THAT'S ALL SIR THANK YOU😇😇
