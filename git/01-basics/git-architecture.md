# Git Architecture

Understanding Git architecture is essential to understanding how Git works internally.

Git works in three main areas:

1. Working Directory  
2. Staging Area  
3. Repository  

---

# 1️⃣ Working Directory

The Working Directory is where you create, edit, or delete files.

It contains the actual files of your project.

Example:
You create or modify a file:

```bash
touch index.html
```

At this stage:
- Git knows the file exists
- But it is NOT saved in Git history yet

---

# 2️⃣ Staging Area (Index)

The Staging Area is a temporary area where you prepare changes before committing.

You move files to staging using:

```bash
git add filename
```

Example:

```bash
git add index.html
```

Now the file is ready to be committed.

Important:
The staging area allows you to choose which changes to commit.

---

# 3️⃣ Repository (.git Folder)

The Repository is where Git permanently stores:

- Commits
- Branch history
- Metadata
- Author information

When you run:

```bash
git commit -m "Added index.html"
```

Git creates a snapshot of the staged changes.

That snapshot becomes part of the repository history.

---

# 🔄 Complete Flow

Working Directory  
        ↓ (git add)  
Staging Area  
        ↓ (git commit)  
Repository  

---

# 📌 Practical Example (Step-by-Step)

## Step 1: Initialize Repository

```bash
git init
```

This creates a hidden `.git` folder.

---

## Step 2: Create File

```bash
touch app.js
```

Check status:

```bash
git status
```

Output:
File is untracked.

---

## Step 3: Add to Staging

```bash
git add app.js
```

Now the file is staged.

---

## Step 4: Commit

```bash
git commit -m "Added app.js file"
```

Now the file is saved permanently in Git history.

---

# 🎯 Why This Architecture Is Powerful

- You control what gets committed
- You can review changes before saving
- You can create clean, logical commits
- You can undo or revert safely

---

# 💡 Important Concept

Git does NOT track files continuously.

It only tracks changes when:
- You add them (git add)
- You commit them (git commit)

Until then, changes exist only in your working directory.

---

# 🧠 Visual Understanding

Think of it like this:

Working Directory = Your Desk  
Staging Area = Files placed in a folder to submit  
Repository = Final submitted record stored permanently  

---

# Summary

Git Architecture consists of:

- Working Directory → Where you work
- Staging Area → Where you prepare
- Repository → Where Git saves history

Understanding this flow is the foundation of mastering Git.
