# Basic Git Commands (With Practical Demo)

This section explains essential Git commands with a small real-life workflow example.

---

# 1️⃣ Initialize a Repository

```bash
git init
```

What it does:
- Creates a new Git repository
- Generates a hidden `.git` folder
- Starts tracking the project

---

# 2️⃣ Check Repository Status

```bash
git status
```

What it shows:
- Modified files
- Untracked files
- Staged files
- Current branch

This is one of the most used Git commands.

---

# 3️⃣ Add Files to Staging Area

Add a single file:

```bash
git add filename
```

Add all files:

```bash
git add .
```

What it does:
Moves changes from Working Directory → Staging Area.

---

# 4️⃣ Commit Changes

```bash
git commit -m "Your message"
```

What it does:
- Creates a snapshot of staged changes
- Saves it permanently in Git history

Important:
Commit only saves staged changes.

---

# 5️⃣ View Commit History

```bash
git log
```

Shows:
- Commit ID
- Author
- Date
- Commit message

Short version:

```bash
git log --oneline
```

---

# 6️⃣ Practical Mini Demo (Step-by-Step)

Let’s simulate a small project.

---

## Step 1: Initialize Project

```bash
mkdir demo-project
cd demo-project
git init
```

---

## Step 2: Create a File

```bash
touch app.js
```

Check status:

```bash
git status
```

Output:
app.js is untracked.

---

## Step 3: Add File

```bash
git add app.js
```

Check again:

```bash
git status
```

Now it shows:
app.js is staged.

---

## Step 4: Commit

```bash
git commit -m "Added app.js file"
```

Now Git has saved the file in its history.

---

## Step 5: Modify File

Edit `app.js`.

Then check status:

```bash
git status
```

Git shows:
File modified.

---

## Step 6: Add & Commit Again

```bash
git add app.js
git commit -m "Updated app.js with new changes"
```

Now you have two commits in history.

Check:

```bash
git log --oneline
```

---

# 🔁 What Just Happened?

You:

1. Initialized Git
2. Created a file
3. Staged it
4. Committed it
5. Modified it
6. Committed again

Git stored two different snapshots of your project.

---

# 🎯 Key Takeaways

- `git init` starts tracking
- `git status` checks state
- `git add` stages changes
- `git commit` saves snapshot
- `git log` shows history

Understanding these commands is the foundation of Git.
