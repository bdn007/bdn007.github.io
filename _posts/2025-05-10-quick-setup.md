---
date: 2025-05-10
title: Quick Setup
---

### If you’ve done this kind of thing before

**https:**  `<https://github.com/<github_account>/repo_name.git>`  
Get started by creating a new file or uploading an existing file. We recommend every repository include a README, LICENSE, and .gitignore.
{: .notice--info}

### …or create a new repository on the command line
```
echo "# <repo_name>" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/<github_account>/<sub_repo_name>.git
git push -u origin main
```

### …or push an existing repository from the command line
```
git remote add origin https://github.com/<github_account>/<repo_name>.git
git branch -M main
git push -u origin main
```