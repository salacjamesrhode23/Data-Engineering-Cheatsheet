#### 1️⃣ Fork the Original Repository
#### Go to the original repository on GitHub and click "Fork" to create a copy under your account.
#### This is your workspace where you can freely make changes.

#### 2️⃣ Clone Your Fork Locally
git clone https://github.com/your-username/forked-repo.git
cd forked-repo
#### This downloads the repository to your machine. You now have a local copy to work on.

#### 3️⃣ Set Up the Original Repo as Upstream
git remote add upstream https://github.com/original-owner/original-repo.git
git fetch upstream
#### 'origin' -> your fork
#### 'upstream' -> original repository
#### This allows you to sync changes from the original repo later.

#### 4️⃣ Create a New Branch for Your Work
git checkout -b feature/my-change
#### Never work directly on main/master.
#### Branch names should describe the feature or fix (e.g., bugfix/login-error, feature/dashboard-ui).

#### 5️⃣ Make Changes / Code
#### Edit files, add features, fix bugs, etc.
#### Test your changes locally.

#### 6️⃣ Stage and Commit Changes
git add .
git commit -m "Add feature X / Fix bug Y"
#### Commit messages should be clear and concise.

#### 7️⃣ Sync With Original Repo (Optional, recommended)
git fetch upstream
git checkout main
git merge upstream/main
git checkout feature/my-change
git rebase main  #### or merge main into your branch
#### Ensures your branch is up-to-date before submitting.

#### 8️⃣ Push Your Branch to Your Fork
git push origin feature/my-change
#### Uploads your branch to your GitHub fork.

#### 9️⃣ Create a Pull Request (PR)
#### Go to your fork on GitHub, click "Compare & pull request".
#### Target repository: original owner's repo.
#### Target branch: usually main or develop.
#### Add description, screenshots, context if needed.
#### Submit PR.

#### 🔟 CI/CD Integration
#### If the original repo has CI/CD (GitHub Actions, Travis, Jenkins):
#### Your PR will trigger automated builds, tests, linting.
#### Fix any failing tests, then push changes to the same branch.
#### PR updates automatically.

#### 1️⃣1️⃣ Merge / Review
#### Maintainers review your PR.
#### They may request changes → update your branch → push again.
#### Once approved, maintainers merge your branch into the original repo.

#### Optional: Keep Your Fork Updated
git fetch upstream
git checkout main
git merge upstream/main
git push origin main
#### Keeps your fork in sync with the original repo for future contributions.
