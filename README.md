# P05-Git-Cherry-Pick-Demo

This repository demonstrates the use of `git cherry-pick` — a powerful Git command used to apply specific commits from one branch onto another, without merging the entire branch.

---

## 🧠 What is Cherry-Pick?

`git cherry-pick <commit>` lets you:

- Copy a specific commit from another branch
- Avoid merging the whole branch
- Keep your commit history clean and intentional

---

## 🛠️ What This Repo Includes

- A `main` branch with the base setup
- A `feature-branch` with a unique commit
- That unique commit was cherry-picked into `main`

---

## 🔁 Steps Performed

1. Created `feature-branch` from `main`
2. Added a file `feature.txt` and committed it. Added another file `latest-feature.txt` and commited it.
3. Switched back to `main`
4. Cherry-picked the commit from `feature-branch` using its hash
5. Verified changes using `git log` and confirmed `feature.txt` appeared in `main`

---

## 📌 Useful Commands

```bash
# View commit history
git log --oneline

# Switch branches
git checkout main

# Cherry-pick a specific commit
git cherry-pick <commit-hash>
