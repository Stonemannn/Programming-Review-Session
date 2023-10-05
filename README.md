# Programming Review Session: Git and GitHub Workflow

Welcome to the Git and GitHub review session! In this session, we'll walk through the basic workflow you'll use for your mid-term projects. 

## Basic Git and GitHub Workflow

### 0. Fork Repository
(One student in each group) Click on the "Fork" button, and create a separate repository for your team. This is the one you will use for the following steps.

### 1. Clone the Repository
Clone the remote repository to your local machine.
```bash
git clone https://github.com/username/repository.git
```

### 2. Navigate to the Repository
Change your directory to the cloned repository.
```bash
cd repository
```

### 3. Pull Latest Changes
Before making any changes, it's a good practice to pull the latest updates from the remote repository. This ensures you're working with the most recent version of the code.
```bash
git pull origin main
```

**Note**: In the newer repositories, the default branch name is `main` instead of `master`. Make sure you're pulling from the correct branch.

### 4. Create a New Branch
Always work on a new branch when adding features or fixing bugs. This keeps the main branch stable.
```bash
git checkout -b new-feature
```

This command creates and checks out the branch in one step.

Check all existing branches (including which one you are on currently):
```bash
git branch
```

### 5. Make Changes
Edit files, write code, fix bugs, and make any necessary changes.

### 5a. Double Check Changes Made
Before you start adding changes to a commit, you want to make sure you didn't accidentally change/remove/add files that shouldn't be there.
Use the following command to check what all files exist in your staging area.
```bash
git status
```

### 6. Stage Changes
Once you're satisfied with your changes, stage them for commit. You can specify individual files or stage all changed files.
```bash
git add [filename]
OR 
git add . (adds every file that shows up when you do git status)
```

### 7. Commit Changes
Commit your staged changes with a meaningful commit message.
```bash
git commit -m "Added new feature"
```
Optional: Double check that your commit was added succesfully and correctly:
```bash
git log (shows all of the logs, in chronological order with commit message and files)
git log --pretty=oneline (shows a short preview of the commit message; useful for quick overview of commits)
```

### 8. Push the Branch to Remote
Push your new branch to the remote repository.
```bash
git push origin new-feature
```

### 9. Create Pull Request on GitHub
Navigate to your GitHub repository in your web browser. Click on the `New Pull Request` button. Choose to merge `new-feature` into `main`.

### 10. Resolve Conflicts on GitHub
If GitHub indicates that there are merge conflicts, you have the option to "Resolve conflicts" within GitHub's interface. Click this button, make the necessary adjustments, and then save.

### 11. Complete Pull Request
After resolving any conflicts, finalize the pull request by merging `new-feature` into `main`.

**Note**: Always ensure that your local branch is up-to-date with the `main` branch before creating a pull request to minimize merge conflicts.

