# Exam plan, 8 to 16 September

One file, no build step. `index.html` is the whole app.

## Put it on GitHub

```bash
mkdir exam-plan && cd exam-plan
# copy index.html and README.md in here
git init
git add .
git commit -m "Study plan and chapter tracker"
git branch -M main
git remote add origin https://github.com/Bekabiz/exam-plan.git
git push -u origin main
```

Create the empty `exam-plan` repo on GitHub first. When git asks for a password, paste a **new** personal access token, not the old one.

## Put it on Vercel

1. vercel.com, New Project, Import the `exam-plan` repo.
2. Framework preset: **Other**. Build command: leave empty. Output directory: leave empty.
3. Deploy.

No config file is needed. Vercel serves `index.html` at the root.

## Notes

- Ticks are stored in the browser that opened the site, so use the same phone or laptop each time.
- "Save a backup file" downloads `exam-progress.json`. "Load a backup file" restores it on another device.
