# Manual Setup and Deployment Instructions

Follow these steps in your terminal to verify and deploy your portfolio.

## 1. Check Installation
Start by verifying your Quarto installation:
```powershell
quarto check
```
If this command runs without errors (prints "OK"), proceed to the next step.

## 2. Local Preview
Preview the site locally to ensure it builds correctly:
```powershell
quarto preview
```
This should launch a browser window showing your site. Press `Ctrl+C` in the terminal to stop the server when done.

## 3. Verify Git Configuration
Check your remote repository connection:
```powershell
git remote -v
```
You should see an output starting with `origin`.
If the output is empty or incorrect, add the remote manually (replace with your actual repo URL if different):
```powershell
git remote add origin https://github.com/UnalKulekci/304.2_MedInf_Portfolio.git
```

## 4. Commit Changes
Save your current work to git:
```powershell
git add .
git commit -m "Initial portfolio setup"
```

## 5. Deploy to GitHub Pages
Finally, publish your site:
```powershell
quarto publish gh-pages
```
This command will build your site and push it to the `gh-pages` branch on GitHub.
