# What is Git?

Git is a Distributed Version Control System (DVCS) used to track changes in source code during software development.

It allows developers to save different versions of their project and go back to any previous version if needed.

---

# What is Version Control?

Version Control is a system that records changes to files over time.

## Real-Life Example

Imagine you are writing an assignment:

- assignment_v1.doc
- assignment_v2.doc
- assignment_final.doc
- assignment_final_latest.doc 😅

Git replaces this messy system.

Instead of creating multiple files, Git keeps track of all versions internally.

---

# Why Git is Important

- Tracks every change
- Prevents accidental deletion
- Allows teamwork
- Supports branching
- Maintains complete history

---

# Centralized vs Distributed Version Control

Centralized (Example: SVN)
- One central server
- Internet required
- If server crashes → risk of data loss

Distributed (Git)
- Every developer has full copy
- Works offline
- Faster performance

---

# Git Architecture

Git has three main areas:

1. Working Directory  
   → Where you create or edit files.

2. Staging Area  
   → Where you prepare files before committing.

3. Repository  
   → Where Git permanently stores history.

Flow:

Working Directory → Staging Area → Repository

---

# Practical Demo Flow (Step-by-Step)

Let’s see how Git works in real life.

## Step 1: Initialize Repository

```bash
git init
```

This creates a hidden `.git` folder.

---

## Step 2: Create a File

Create a file:

```bash
touch index.html
```

Check status:

```bash
git status
```

Git will show the file as untracked.

---

## Step 3: Add to Staging Area

```bash
git add index.html
```

Now the file is staged.

---

## Step 4: Commit Changes

```bash
git commit -m "Added index.html file"
```

Now the file is saved permanently in Git history.

---

# What Just Happened?

You:

- Created a file
- Added it to staging
- Saved a snapshot (commit)

This commit acts like a version checkpoint.

You can go back anytime using Git history.

---

# Important Concept

A commit is not just saving a file.

It is saving:
- Changes
- Author info
- Timestamp
- Commit message
- Unique commit ID (hash)

---

# Who Created Git?

Git was created by Linus Torvalds in 2005 to manage the Linux kernel project.
