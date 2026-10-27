# Git Commands Checklist

Use these commands after creating an empty GitHub repository.


```bash
git remote add origin https://github.com/cgoudar-sys/flask-git-assignment.git
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
