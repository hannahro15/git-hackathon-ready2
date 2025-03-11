# README: How to Collaborate on a GitHub Project

## 📌 Introduction
Git and GitHub are essential tools for developers working in teams. Learning how to collaborate using these tools is a crucial step in your journey as a developer. Whether you're contributing to open-source projects or working on a team, understanding GitHub collaboration helps you work efficiently and keep track of changes.

If you're taking your first steps into Git collaboration, congratulations! This is a big milestone, and you should be proud of yourself for learning these skills. Every great developer started where you are now, and the more you practice, the more confident you'll become.

This guide explains how to contribute to a GitHub project, step by step. Follow these instructions to fork, clone, make changes, and submit a pull request.

---
# How to collaborate in a GitHub project:
- Review collaboration policy in the project
- Fork the repo
- Clone forked repo
- Update master branch
- Create a branch
- Make our improvements
- Create a pull request
- Sync a fork
- Rebasing a pull request




## 🔍 Step 1: Understand the Project Rules
Before contributing, check the project's collaboration guidelines. Some projects have specific rules for submitting changes.

---

## 🔄 Step 2: Fork the Repository
A "fork" is your own copy of the project. To create one:
- Go to the project on GitHub.
- Click **Fork** (top right corner). This creates a copy under your account.

Example repo: [Git-Hackathon-Ready](https://github.com/LaneSawyerT/git-hackathon-ready2)

---

## 💾 Step 3: Clone Your Fork
Cloning downloads the repository to your computer.
```sh
    git clone https://github.com/YOUR-USERNAME/gazelle-analyser-api.git

    Replace YOUR-USERNAME with your GitHub username
```


## 🔗 Step 4: Link the Original Repository
This ensures you can update your copy with new changes from the main project.
```sh
    git remote add upstream https://github.com/jmsampayo/gazelle-analyser-api.git
    git remote -v
```

You should now see two remotes:

origin (your fork)

upstream (the original repo)

## 📥 Step 5: Keep Your Branch Updated

Before making changes, update your local project.
```sh
git checkout master
git pull upstream master
```

## 🌿 Step 6: Create a New Branch

A branch keeps your changes separate until they are ready.
```sh
git checkout -b my-new-feature
```

## ✏️ Step 7: Make and Save Changes

Edit files in your project, then check what changed:
```sh
git status
```
Add your changes and commit them:
```sh
git add .
git commit -m "Added a new feature"
```
Push your changes to GitHub:
```sh
git checkout -b my-new-feature
```

## 🔀 Step 8: Create a Pull Request (PR)

A pull request asks the project owner to review and merge your changes.

Go to your fork on GitHub.

Click Compare & pull request.

Write a description of your changes.

Click Create pull request.

If possible, link your PR to an open issue.


## 🔃 Step 9: Sync Your Fork (Keeping It Updated)

If the main project changes, update your fork:
```sh
git fetch upstream
git checkout master
git merge upstream/master
```
This ensures you are working with the latest version.

## 🛠️ Step 10: Rebase Your Pull Request (If Needed)

If your pull request has conflicts, you may need to rebase:
```sh
git checkout my-new-feature
git rebase upstream/master
```
If necessary, force push your updated branch:


## 🔄 Step 11: Squash Multiple Commits (If Required)

Sometimes, project maintainers prefer a single clean commit. To squash the last 5 commits into one:
```sh
git reset --soft HEAD~5
git commit -m "Refactored code and improved feature"
git push origin +my-new-feature
```
The + sign forces a push with rewritten history.





## ✅ Additional Tips

Keep your PRs small and focused.

Write clear commit messages.

Be open to feedback and improve your code if requested.



🎉 Keep going, and enjoy learning GitHub collaboration! Every contribution you make helps improve a project and builds your confidence as a developer.



















