# Git Security Best Practices – What I Did

## 01. I initialized the Git repository  
![Screenshot of terminal showing `git init`](screenshots/01-git-init.png)

---

## 02. I created a `.gitignore` file to ignore sensitive files like `.env`  
![Screenshot of VS Code showing `.gitignore` file](screenshots/02-gitignore-file.png)

---

## 03. I confirmed that `.env` was successfully ignored by Git  
![Screenshot of terminal showing `.env` is not tracked](screenshots/03-env-not-tracked.png)

---

## 04. I created a `pre-commit` hook to block secrets (like `sk-test`)  
Then I tried committing a secret, and Git **blocked** the commit  
![Screenshot of terminal showing commit blocked by hook](screenshots/04-secret-commit-blocked.png)

---

## 05. I removed the secret and made a clean commit  
![Screenshot of terminal showing successful commit](screenshots/05-clean-commit.png)

---

## 06. I pushed the code to GitHub successfully  
![Screenshot of terminal showing successful `git push`](screenshots/06-git-push-success.png)

---

## Final Result  
- Sensitive files like `.env` are ignored  
- Pre-commit hook blocks secret keys like `sk-test`  
- Clean commits are allowed and pushed to GitHub safely

---

