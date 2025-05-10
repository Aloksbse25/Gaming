git --version - # Check Git version (all OS)  -   
# Example output: git version 2.40.0 

# Configure Git (global settings)  
git config --global user.name "Your Name"  
git config --global user.email "your@email.com"  

GitHub Git Cheat Sheet Code Collection 

# INSTALLATION & GUIS

# SETUP
# Configure user information
git config --global user.name "[firstname lastname]"
git config --global user.email "[valid.email]"
git config --global color.ui auto

# SETUP & INIT
# Initialize or clone repositories
git init
git clone [url]

# STAGE & SNAPSHOT
# Working with changes and commits
git status
git add [file]
git reset [file]
git diff
git diff --staged
git commit -m "[descriptive message]"

# BRANCH & MERGE
# Branching and merging workflows
git branch
git branch [branch-name]
git checkout [branch-name]
git merge [branch]
git log

# INSPECT & COMPARE
# Examining changes and history
git log branchB...branchA
git log --follow [file]
git diff branchB...branchA
git show [SHA]

# TRACKING PATH CHANGES
# Managing file movements
git rm [file]
git mv [existing-path] [new-path]
git log --stat -M

# IGNORING PATTERNS
# Excluding files from version control
# Create .gitignore file with patterns like:
# logs/
# *.notes
# pattern*/
git config --global core.excludesfile [file]

# SHARE & UPDATE
# Working with remotes
git remote add [alias] [url]
git fetch [alias]
git merge [alias]/[branch]
git push [alias] [branch]
git pull

# REWRITE HISTORY
# Modifying commit history
git rebase [branch]
git reset --hard [commit]

# TEMPORARY COMMITS
# Stashing changes
git stash
git stash list
git stash pop
git stash drop