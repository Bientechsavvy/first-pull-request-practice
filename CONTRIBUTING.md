# How to open your first pull request

Follow these steps in order. Do the browser route if you don't have Git installed.

## 1. Fork the repository
Click **Fork** at the top right of the repo page, then **Create fork**. You now have your own copy.

## 2. Get the files
**Option A: on your computer**
```bash
git clone https://github.com/Bientechsavvy/first-pull-request-practice
cd first-pull-request-practice
```
**Option B: in the browser**: press `.` (the full stop key) on your fork's page to open the web editor.

## 3. Create a branch
```bash
git switch -c add-your-name-here
```
Use a short, descriptive name like `add-ada-about-me`.

## 4. Make your change
1. Copy `about-me/TEMPLATE.md` to `about-me/your-github-username.md`.
2. Fill it in. Keep it friendly and appropriate for everyone.
3. Add your name to `CONTRIBUTORS.md`.

## 5. Commit your work
```bash
git add .
git commit -m "Add about-me file for YOUR-USERNAME"
```

## 6. Push to GitHub
```bash
git push -u origin add-your-name-here
```

## 7. Open the pull request
Go to your fork on GitHub and click **Compare & pull request**. Write a short title and description, then click **Create pull request**.

## 8. Celebrate 🎉
A maintainer will review and merge it. You have now made your first contribution!

## Common problems
 Problem => Fix 

 `fatal: not a git repository` => You are in the wrong folder. Use `cd` to enter the project folder.
 `Permission denied` on push | Check you cloned **your fork**, not the original repo.
 `nothing to commit` => Save your file first, then run `git add .` again.
 Merge conflict => Open the file, keep the lines you want, delete the `<<<<`, `====`, `>>>>` markers, then add and commit.
 Pushed to the wrong branch => Create a new branch from where you are and push that one.

## Commit message tips
- Start with a verb: "Add", "Fix", "Update".
- Keep it short and specific.
