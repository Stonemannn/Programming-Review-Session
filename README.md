# Programming-Review-Session

In this session, we are going to walk through the basic git and github workflow for your mid-term projects.

Here is the simplified workflow:

**Clone the Repository**: Clone the remote repository to your local machine.
   ```bash
   git clone https://github.com/username/repository.git
   ```

**Navigate to the Repository**: Change directory to the cloned repository.
   ```bash
   cd repository
   ```

**Pull Latest Changes**: It's a good practice to pull the latest changes from the remote repository to make sure you're working with the most recent version.
   ```bash
   git pull origin master
   ```

**Create a New Branch**: Create a new branch for your work.
   ```bash
   git branch new-feature 
   git checkout new-feature
   ```

**Make Changes**: Edit files and make your changes.

**Stage Changes**: Stage your changes for commit. You can specify the changed files you want to stage, or all changed files.
   ```bash
   git add .
   ```

**Commit Changes**: Commit your staged changes.
   ```bash
   git commit -m "Added new feature"
   ```

**Push the Branch to Remote**: Push your new branch to the remote repository.
   ```bash
   git push origin new-feature
   ```

**Create Pull Request on GitHub**: Go to your GitHub repository and create a new pull request. Choose to merge `new-feature` into `master`.

**Resolve Conflicts on GitHub**: If GitHub indicates that there are conflicts, you will have an option to "Resolve conflicts" right on GitHub's interface. Click that button, make the necessary adjustments, and then save.

**Complete Pull Request**: Once conflicts are resolved, you can complete the pull request by merging `new-feature` into `master`.

In this workflow, the entire process of resolving conflicts is handled on GitHub, without requiring any local conflict resolution.
