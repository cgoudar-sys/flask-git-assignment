# Git Commands Checklist

Use these commands after creating an empty GitHub repository.

Replace `YOUR_USERNAME` with your GitHub username.

```bash
git remote add origin https://github.com/YOUR_USERNAME/flask-git-assignment.git
git push -u origin main
git push -u origin dev
```

To check the branch and commit history:

```bash
git branch
git log --oneline --graph --all
```

Expected branch workflow:

```text
dev  -> Version 1 commit -> Version 2 commit
main <- merge Version 1 <- merge Version 2
```
