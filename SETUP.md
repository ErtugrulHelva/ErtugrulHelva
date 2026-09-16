# Setup Guide

## 1. Create the special profile repo
On GitHub, create a new repo with the **exact same name as your username** (e.g. `ErtugrulHelva/ErtugrulHelva`). Make it public. GitHub will automatically display this repo's README on your profile page.

## 2. Edit README.md
Fill in the remaining placeholders in `README.md` (`[your areas of expertise]`, `[a short fun fact]`, etc.) with your own info. Feel free to remove sections you don't need (e.g. snake animation, trophy, stats).

## 3. Push the files to the repo
```bash
cd ~/github-profile
git init
git remote add origin https://github.com/ErtugrulHelva/ErtugrulHelva.git
git add .
git commit -m "Add profile README"
git branch -M main
git push -u origin main
```

## 4. (Optional) Enable the snake animation
As long as `.github/workflows/snake.yml` exists in the repo, GitHub Actions will run automatically and generate an SVG on the `output` branch. No extra config needed, just:
- Go to **Settings → Actions → General → Workflow permissions** and set it to **"Read and write permissions"**.
- To trigger the first run manually: **Actions** tab → *Generate Snake Animation* → **Run workflow**.

## 5. Verify the stats cards work
`github-readme-stats` and `streak-stats` services can sometimes be slow or time out under load. If you run into issues:
- Refresh the page a few times.
- Alternatively, deploy these services on your own Vercel account and update the URLs accordingly (see https://github.com/anuraghazra/github-readme-stats).

## 6. Checklist
- [ ] Repo name = GitHub username
- [ ] All remaining placeholders in README filled in
- [ ] Social/email links updated
- [ ] Unwanted sections removed
- [ ] Pushed and visible on your profile (github.com/ErtugrulHelva)
