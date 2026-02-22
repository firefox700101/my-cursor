# Sync this project to GitHub

## 1. Turn this folder into a Git repo

In Terminal (or Cursor’s integrated terminal), run:

```bash
cd /Users/zhang2000/learn/my-cursor
git init
```

## 2. Create a repo on GitHub

1. Go to [github.com](https://github.com) and sign in.
2. Click **“+”** → **“New repository”**.
3. Name it (e.g. `my-cursor`), choose public/private, **do not** add a README (you already have files).
4. Click **“Create repository”**.

## 3. Connect this folder to GitHub

GitHub will show commands; use these (replace `YOUR_USERNAME` with your GitHub username):

```bash
git remote add origin https://github.com/YOUR_USERNAME/my-cursor.git
```

## 4. Edit or add files

- Edit `ibm.txt` or any file in Cursor as usual (File → Open, or open from the sidebar).
- Create new files in the `my-cursor` folder; they will show up in Git once you add them.

## 5. Commit and push to GitHub

Each time you want to save your changes to GitHub:

```bash
cd /Users/zhang2000/learn/my-cursor

# Stage files (all changes, or specify files)
git add .
# Or:  git add ibm.txt   (only that file)

# Commit with a message
git commit -m "Describe your changes"

# Push to GitHub (first time: set upstream)
git push -u origin main
```

If your default branch is `master` instead of `main`, use:

```bash
git push -u origin master
```

## 6. Later: just push

After the first push, you only need:

```bash
git add .
git commit -m "Your message"
git push
```

---

**Tip:** Install the “cursor” command in your PATH (**Cmd+Shift+P** → *Shell Command: Install 'cursor' command in PATH*) so you can open this folder from Terminal with `cursor /Users/zhang2000/learn/my-cursor`.
