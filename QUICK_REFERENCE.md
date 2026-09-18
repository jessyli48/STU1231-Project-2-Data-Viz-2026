# Git Quick Reference (When You Forget)

Copy-paste these commands. Replace words in `[brackets]` with your actual values.

---

## 🚀 FIRST TIME ONLY (Setting Up)

```bash
git clone https://github.com/[YOUR-USERNAME]/climate-viz.git
cd climate-viz
code .
```

---

## 📝 EVERY TIME YOU WORK (The Three Commands)

**Step 1: See what you changed**
```bash
git status
```
(Shows which files changed)

**Step 2: Save your work**
```bash
git add .
```
(The `.` means "all files I changed")

**Step 3: Label it**
```bash
git commit -m "Describe what you changed here"
```

**Step 4: Upload to GitHub**
```bash
git push
```

**All together (what you'll do most):**
```bash
git add .
git commit -m "Add interactive map with climate data"
git push
```

---

## 📥 GETTING AIDEN'S CHANGES

If Aiden pushed changes and you want them:

```bash
git pull
```

Do this before you start working to avoid conflicts.

---

## 🐛 YOU MESSED UP (Common Mistakes)

### "I committed but haven't pushed yet"
```bash
git reset HEAD~1
```
(Undoes last commit, keeps your changes)

### "I pushed something wrong"
```bash
git revert HEAD~1
git push
```
(Creates a new commit that undoes the old one)

### "I deleted a file by accident"
```bash
git checkout HEAD [filename]
```

### "I want to see what I've done"
```bash
git log
```
(Shows your commit history)

### "Aiden and I edited the same file and there's a conflict"
Text Jessy or Aiden—it's fixable. Don't panic.

---

## 📊 SEE YOUR PROGRESS

```bash
git log --oneline
```
Shows all your commits in a clean list.

---

## 🚀 DEPLOYING TO THE WEB

Once you push, your site automatically updates at:
`https://[YOUR-USERNAME].github.io/climate-viz/`

(No extra commands needed! Push to GitHub = instant website update)

---

## 💡 THE WORKFLOW IN ONE IMAGE
Edit files in VS Code
↓
git add .
↓
git commit -m "message"
↓
git push
↓
Check GitHub → website updates automatically


That's the whole thing. Repeat forever.

---

## 🎯 WHAT NOT TO DO

❌ Don't put large data files in Git (use Google Drive)
❌ Don't edit files on GitHub directly
❌ Don't push without a commit message
❌ Don't panic if something breaks—everything is recoverable

---

## 👥 WORKING WITH AIDEN

1. **Before you start:** `git pull` (get her latest changes)
2. **Do your work:** Edit files
3. **When done:** `git add .` → `git commit -m "..."` → `git push`
4. **Aiden does same:** She pulls your changes, does her work, pushes

---

**Bookmark this file. Refer to it constantly. You'll be fine.** 🚀