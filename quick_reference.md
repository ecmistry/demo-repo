# GitHub Workflow - Quick Reference Card

## Complete Workflow (30-second version)

```bash
# 1. Clone repo
git clone https://github.com/ORG/REPO.git && cd REPO

# 2. Create feature branch
git checkout -b feature/my-feature

# 3. Make changes (edit files)

# 4. Stage changes
git add .

# 5. Commit
git commit -m "Add new feature"

# 6. Push to remote
git push -u origin feature/my-feature

# 7. Create PR on GitHub (via web UI)

# 8. Merge PR on GitHub (via web UI)

# 9. Update local main
git checkout main && git pull origin main

# 10. Clean up
git branch -d feature/my-feature
```

## Key Explanations to Give

**Git Clone**: Creates local copy of remote repository  
**Checkout -b**: Creates AND switches to new branch  
**Git Add**: Stages changes (prepares for commit)  
**Git Commit**: Creates snapshot of staged changes  
**Git Push**: Uploads local commits to GitHub  
**Pull Request**: Formal request to merge with code review  
**Git Pull**: Downloads and merges remote changes  

## Common Interview Questions

**Q: Difference between git fetch and git pull?**  
A: Fetch downloads changes without merging. Pull = fetch + merge.

**Q: What's a merge conflict?**  
A: When same lines are changed in different branches. Must manually resolve.

**Q: Why use branches?**  
A: Isolate changes, enable parallel work, safer code review process.

**Q: Git reset vs git revert?**  
A: Reset rewrites history (use locally). Revert creates new commit (use on shared branches).

## Emergency Commands

```bash
git status                    # Where am I?
git log --oneline            # What happened?
git branch                   # What branches exist?
git restore file.txt         # Undo unstaged changes
git restore --staged file.txt # Unstage file
```
