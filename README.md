# Company-Sales-Performance-Dashboard

# Tableau Project

This repository contains a Tableau **packaged workbook** (`.twbx`) so it’s easy to download and open without setting up data connections.

## Contents
- `tableau/Tablueaiu Project.twbx` — the packaged workbook
- `.gitattributes` — routes `.twbx` files through Git LFS if you enable it
- `.gitignore` — ignores temp/system files

## How to open
1. Download the `.twbx` from this repo.
2. Open it with **Tableau Desktop** or free **Tableau Reader**.

## Screenshots (optional)
Add a `/screenshots` folder with a few PNGs so people can preview your dashboards on GitHub.

## How to use this repo
- If your `.twbx` is **over 100 MB** (current size: **0.37 MB**), you should use **Git LFS** before pushing.
- See the steps below.

## Publish steps (CLI)
```bash
# 1) Initialize (run in this folder)
git init
git add -A
git commit -m "Add Tableau packaged workbook"

# 2) (Recommended) enable Git LFS for Tableau packages
git lfs install
git lfs track "*.twbx"
git add .gitattributes
git commit -m "Track .twbx with Git LFS"

# 3) Create a new repo on GitHub, then add it as remote and push
git remote add origin https://github.com/<your-username>/<repo-name>.git
git branch -M main
git push -u origin main
```
