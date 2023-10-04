# Programming Review Session: Git and GitHub Workflow

Welcome to the Git and GitHub review session! In this session, we'll walk through the basic workflow you'll use for your mid-term projects. 

## Basic Git and GitHub Workflow

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

### 5. Make Changes
Edit files, write code, fix bugs, and make any necessary changes.

### 6. Stage Changes
Once you're satisfied with your changes, stage them for commit. You can specify individual files or stage all changed files.
```bash
git add .
```

### 7. Commit Changes
Commit your staged changes with a meaningful commit message.
```bash
git commit -m "Added new feature"
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
