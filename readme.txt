1. Fork the Repository
- Go to BookStack GitHub Repo and click Fork.
- This creates a copy under your own GitHub account (yourname/BookStack).

2. Clone Your Fork Locally
- git clone https://github.com/yourname/BookStack.git
- cd BookStack

3. Add the Original Repo as an "Upstream" Remote
This lets you pull updates from the official source later:
- git remote add upstream https://github.com/BookStackApp/BookStack.git
- git fetch upstream

4. Create a New Branch for Your Custom Work
- git checkout -b my-custom-version

5. Commit & Push Your Custom Code
- git add .
- git commit -m "My custom changes"
- git push origin my-custom-version

Later, When a New Version is Released (e.g., after 1–2 years)
6. Fetch the Latest Changes from Original Repo
- git checkout main
- git pull upstream main

7. Merge Updates Into Your Custom Branch
- git checkout my-custom-version
- git merge main

Git will try to merge automatically.
If there are conflicts, Git will notify you. You'll need to resolve them manually in each file.
After resolving:

- git add .
- git commit -m "Merge updates from upstream/main"