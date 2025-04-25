# About-Git
This repository contains a basic introduction to Git, including installation, essential commands, working with branches, and connecting with GitHub. Perfect for beginners.

🧠 What is Git?
Git is like a save button for your code, but way cooler.
It:
- Remembers every change you make
- Lets you go back if you mess up
- Helps you and your friends work on the same project without stepping on each other’s toes


🎯 Why Do We Use Git?
Because:
- You don’t want to lose your work
- You want to fix mistakes easily
- You want to work together on code with others, and Git keeps it all organized


**🛠️ Getting Started**
Before using Git, tell it who you are:

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

**📁 Step 1: Make a New Project (Repository)**
Think of a "repo" like a folder that Git watches.

```bash
mkdir my-project         # Make a folder
cd my-project            # Go into that folder
git init                 # Tell Git to start watching this folder
```

**🌍 Step 2: Connect to GitHub**
GitHub is like a home for your code on the internet.

1. Go to [github.com](https://github.com)
2. Click New repository
3. Name it (like `my-first-repo`)
4. Copy the link (it ends with `.git`)

Now connect your computer to GitHub:

git remote add origin https://github.com/yourname/my-first-repo.git

**🌿 Step 3: Make a New Branch (Like a Playground)**

```bash
git checkout -b my-branch-name
```

This makes a copy of your project so you can try new things without messing up the original.

**💾 Step 4: Save and Share Your Work**
1. Stage your work (tell Git what to save):

```bash
git add .
```

2. Save it (commit):

```bash
git commit -m "I made some changes"
```

3. Send it to GitHub:

```bash
git push origin my-branch-name
```

**🔄 Step 5: Get the Latest Changes**
If someone else made updates, grab them:

```bash
git pull origin main
```

🧹 Other Helpful Stuff
- `git status` – shows what changed
- `git log` – shows a list of saves (commits)
- `git checkout main` – go back to the main version
- `git merge my-branch` – mix your branch into the main project


**📂 Pushing a New Branch to GitHub (First Time)**

When you create a new branch in your IDE (like `new-feature`), it only exists on your computer. To make it show up on GitHub, you need to **push** it there.

But before you can do that, you need to **tell Git** where to send this branch on GitHub. This is called **setting the upstream**.

### How to Do It:
Run this command the **first time** you push your new branch:

```bash
git push --set-upstream origin new-feature
 or
git push -u origin new-feature
```

### What Does This Do?
- **push**: Sends your branch to GitHub
- **-u**: Tells Git to remember where to push this branch next time
- **`origin`**: Your GitHub repo
- **`new-feature`**: The name of your branch

After you do this once, you can just run:

```bash
git push
```
