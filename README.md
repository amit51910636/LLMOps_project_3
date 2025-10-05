```
**Project Document Link:** https://docs.google.com/document/d/1VlHirN62sWE1CwXr4v2YM40sg8luskD6VY4A2gKOHK4/edit?usp=sharing
```

doskey /history

pip install uv
uv --version
uv venv
C:\LearnTechWithMeAndAI\code\llmops\project3-llmops\automated-research-report-generation\.venv\Scripts\activate.bat
uv add -r requirements.txt 
or
uv add -r requirements.txt --dev

uv pip list
uv pip show langgraph
uv add ipykernel
uv python list
= use cpython as it is fast compared to pypython



git remote set-url origin https://github.com/amit51910636/LLMOps_project3.git
git remote -v
git push -u origin main

git add .
git commit -m "Add research notebook and exceptions module"
git push origin main
git remote -v


git checkout main
git fetch upstream
git merge upstream/main
git add .
git commit -m "Merged changes from upstream/main"
git push origin main


git remote set-url --push upstream no_push
git remote -v
= origin  https://github.com/amit51910636/LLMOps_project3.git (fetch)
= origin  https://github.com/amit51910636/LLMOps_project3.git (push)
= upstream        https://github.com/sunnysavita10/automated-research-report-generation.git (fetch)
= upstream        no_push (push)
= it wont push to sunny sir repo


5-oct
git config --global --add safe.directory C:/LearnTechWithMeAndAI/code/llmops/project3-llmops/automated-research-report-generation
git config --global --get-all safe.directory
git remote -v
git push -u origin main
git remote add sunny https://github.com/sunnysavita10/automated-research-report-generation.git


git remote remove sunny
git remote -v
git fetch upstream
git merge upstream/main
git checkout main
git merge upstream/main
git push origin main



Option 1: Commit your changes
git add .
git commit -m "Save local changes before merging upstream"
git merge upstream/main

git stash push -m "Temp stash before merging upstream"
git stash push -u -m "Temp stash including untracked file"
git merge upstream/main
git stash pop
doskey /history


git rm --cached .env
echo ".env" >> .gitignore
git add .gitignore
git commit -m "Ignore .env file"
git push origin main


git remote -v
git reset HEAD~1
git restore --staged .env 

"view - command pallate = reload window = or crtl+shift+p"
select text and shift quote to quote whole text

git branch backup-main


-----------

git remote set-url origin https://github.com/amit51910636/LLMOps_project_3.git
git remote -v
git push -u origin main


---------------
You cannot add another origin with the same name. Instead, you should update the existing origin to point to your new GitHub repo.
git remote set-url origin https://github.com/amit51910636/LLMOps_project_3.git

"Step 1: Add Sunny’s repo as upstream"
git remote add upstream https://github.com/sunnysavita10/automated-research-report-generation.git

"Step 2: Verify remotes"
git remote -v

"Use no_push for upstream if you want to ensure you never push to Sunny’s repo by mistake:"
git remote set-url --push upstream no_push

"Step 3: Fetch changes from upstream"
This will download all branches from Sunny’s repo so you can merge/rebase as needed.
git fetch upstream

"Step 4: Merge or rebase changes from upstream"

For example, to merge Sunny’s main branch into your main:
git checkout main

git merge upstream/main
