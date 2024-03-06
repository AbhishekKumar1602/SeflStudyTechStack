# Git and GitHub
Git is a distributed version control system that allows developers to track changes in their code, collaborate with others, and manage different versions of their projects. It's especially useful for managing source code and text files.

GitHub, on the other hand, is a web-based platform that provides hosting for Git repositories. It offers a user-friendly interface for collaborating on software projects, managing code repositories, tracking issues, and facilitating team collaboration. GitHub makes it easier for developers to work together and share their code with the broader community.


## Git: A Version Control System
Git is a distributed version control system used in software development to track changes in source code and manage collaborative projects. It was created by Linus Torvalds in 2005 and has since become an essential tool for developers. Features of Git:

**1. Version Control:**
   - Git allows developers to track changes in their code over time, maintaining a history of every change made to a project. This enables reverting to previous code states, tracking contributors, and understanding the project's evolution.

**2. Distributed System:**
   - Git is a distributed version control system. Each developer working on a project has a complete copy of the repository on their local machine. This decentralization allows for offline work and supports collaboration without relying on a central server.

**3. Snapshot-Based:**
   - Git adopts a snapshot-based approach rather than tracking individual changes. It records the entire project state at each point in time, making it fast, efficient, and safeguarding against data loss.

**4. Branching and Merging:**
   - Git facilitates branching, which creates independent lines of development. Developers can work on features or bug fixes in isolation by creating and switching between branches. Merging combines changes from one branch into another.

**5. Commit:**
   - A commit in Git represents a snapshot of the project at a specific time. Each commit has a unique identifier, a message describing the changes, and references to the previous commit(s). Commits are the foundation of a Git repository.

**6. Staging Area:**
   - Git employs a staging area (index) to selectively choose which changes to include in the next commit. This allows developers to review and fine-tune their changes before committing them.

**7. Remote Repositories:**
   - Git supports remote repositories, which are copies of the project stored on other servers. Developers can push changes to remote repositories and pull changes from them. Platforms like GitHub and GitLab host remote Git repositories.

**8. Collaboration:**
   - Git facilitates collaboration by allowing multiple developers to work on the same project concurrently. They can commit changes locally and then push them to a shared remote repository, making it easy to integrate everyone's work.

**9. Version History:**
   - Git maintains a complete version history of a project, making it easy to track changes, understand their origins, and review their timeline. This is crucial for debugging, auditing, and comprehending the project's development.

**10. Open Source and Extensible:**
   - Git is open source, and there are various tools and graphical user interfaces available to enhance its functionality. It can be integrated into different development workflows and integrated development environments (IDEs).

## Git Installation

 **On MacOS:** To install Git on MacOS, you can use Homebrew with the following command:
```
brew install git
```
**On Linux:** To install Git on Linux, you can use the package manager (e.g., APT on Debian-based systems) with this command:
```
sudo apt-get install git
```

### Creating a Version of a Repository
Creating a Git version of an existing local directory (repository) involves initializing a Git repository in that directory and then committing your files to it.

1. **Initialize a Git Repository:** Use the `git init` command to create a new Git repository in your local directory. This command sets up the necessary Git files and data structures.

    ```
    git init
    ```

2. **Checking Status:** The `git status` command is used in the Git version control system to display the status of your working directory with respect to the Git repository. It provides information on:

    - Untracked Files: Files in your working directory that are not currently being tracked by Git.
    - Changes to be Committed: Files that have been modified and staged for the next commit.
    - Changes not Staged for Commit: Files that have been modified but not yet staged.

    ```
    git status
    ```

3. **Add Files or Folders to the Staging Area:** Use the `git add` command to stage the files or folders you want to include in your initial commit. You can specify the files or folders individually or use wildcard characters to add multiple files at once. To add all files and directories in the current directory:

    ```
    git add .
    ```

    To add specific files or folders, use double quotes for filenames with spaces:

    ```
    git add Sample.txt "Sample Folder"
    ```

4. **Remove Files or Folders from the Staging Area:** Use the `git reset` command to unstage files or folders from the staging area that you do not want to include in your initial commit. You can specify the files or folders individually or use wildcard characters to unstage multiple files at once. To unstage all files and folders in the current directory:

    ```
    git reset .
    ```

    To unstage specific files or folders:

    ```
    git reset Sample.txt "Sample Folder"
    ```

5. **Commit the Staged Changes:** The `git commit` command is used to save your changes to the Git repository. It records a snapshot of the changes you have staged (using `git add`) and creates a new commit with a message describing the changes. The commit message should be a concise description of the changes you are committing.

    ```
    git commit -m "Our Commit Message"
    ```

   In other words, "commit" creates a version, and "Our Commit Message" serves as the version name. If you want to amend the same version, you can use:

   ```
   git commit -m "Our Commit Message" --amend
   ```

### Viewing and Working with Previous Versions of the Repository

1. **Check Git Logs:** The git log command in Git is used to view the commit history of a Git repository. When you run git log, Git will display a list of commits, starting with the most recent commit and working backward in time. Each commit is accompanied by information such as the commit hash, author, date, and commit message.

   ```
   git log
   ```
   This will display a commit history that includes the following information for each commit:
   - Commit Hash: A unique identifier for each commit.
   - Author: The name and email address of the person who made the commit.
   - Date: The date and time the commit was made.
   - Commit Message: The message describing the purpose of the commit.

   - To display a graphical representation of the commit history in a Git repository
   ```
   git log --graph --oneline --all --decorate
   ```
   - `--graph`: Draws a text-based graph of the commit history.
   - `--oneline`: Condenses the commit information to one line per commit.
   - `--all`: Shows all branches, not just the currently checked out one.
   - `--decorate`: Adds extra information, such as branch and tag names.

2. **Using commit-hash to View  and Work with Different Versions**

   A. **Using "git checkout":** Using the `git checkout <commit-hash>` command in Git allows you to switch to a specific commit, effectively taking our repository to the state it was in at that commit.
   ```
   git checkout <commit-hash>
   ```
   B. **Using "git show":** The `git show <commit-hash>` command allows us to view the changes introduced by a specific commit. We can use it to inspect the details of a particular commit.
   ```
   git show <commit-hash>
   ```

   - It can also be used to view files as they existed in a specific commit without changing your working directory, you can use the git show command with a specific file path and commit hash.
      ```
      git show <commit-hash>:path/to/file
      ```

   C. **Using "git reset":** The git reset command in Git allows you to reset your current branch and working directory to a designated commit.
   ```
   git reset <commit>
   ```
   - Options to control how the staging area and working directory are reset.

   - `--soft`: Keeps changes in the working directory and staging area.
   - `--mixed`: Keeps changes in the working directory but resets the staging area.
   - `--hard`: Discards changes in both the working directory and staging area.
   - To undo the last commit and keep changes in the working directory and staging area.
      ```
      git reset --soft HEAD^
      ```
   **NOTE:** Remember to use caution with git reset since it can alter the commit history. If you've already pushed commits to a remote repository, it's generally not recommended to use git reset on shared branches, as it can cause synchronization issues for collaborators. In such cases, it's better to use git revert.


## Useful Miscellaneous Git Commands

**Set Global Aliases**
- For commit -m
```
git config --global alias.cm "commit -m"
```

- To see our git aliases
```
git config --global --get-regexp alias
```

**Temporarily Save Changes**
- Stashing is a method in Git used to temporarily save changes that you prefer not to commit immediately.
```
git stash
```
- Stash Changes with Message
```
git stash save "Stash Message"
```
- List All Stash
```
git stash list
```
- Apply the Latest Stash
```
git stash apply
```
- Apply a Specific Stash
```
git stash apply stash@{n}
```   
- Delete Stash
```
git stash drop stash@{n}
```
- Apply and Drop Latest Stash
```
git stash pop
```
- Clear All Stash
```
git stash clear
```




## GitHub
GitHub is a web-based platform and a powerful tool for version control, collaboration, and project management. It's widely used for hosting and managing software development projects, but its capabilities extend beyond code repositories. Here's a detailed explanation of GitHub:

1. **Version Control System (VCS):**
   - GitHub primarily serves as a Git repository hosting service.
   - Git is a distributed version control system that allows developers to track changes in their codebase over time.

2. **Git Repositories:**
   - On GitHub, a repository (or repo) is a place to store your project's code.
   - It contains all the project files, revision history, and documentation.

3. **Collaboration:**
   - GitHub makes collaboration easy.
   - Multiple users can work on the same project simultaneously.
   - Features like pull requests allow contributors to propose changes, discuss them, and get them merged into the main codebase.

4. **Issues and Bug Tracking:**
   - GitHub provides an issue tracking system.
   - Users can report and discuss bugs, feature requests, and other project-related tasks.

5. **Wiki and Documentation:**
   - Repositories on GitHub can have wikis for documentation.
   - Useful for maintaining project documentation, guidelines, and instructions.

6. **GitHub Pages:**
   - GitHub Pages is a feature that allows you to publish web content directly from your repository.
   - It's commonly used for hosting documentation, blogs, or simple websites.

7. **Forks and Pull Requests:**
   - Users can fork a repository, making a copy in their GitHub account.
   - They can propose changes to the original repository through a pull request.

8. **Branching and Workflow:**
   - GitHub supports various branching strategies.
   - Teams can use feature branches, release branches, and more to manage the development process.

9. **Security and Permissions:**
   - GitHub provides fine-grained access control.
   - Repository owners can define who has read and write access, and who can merge changes.

10. **Integrations and Actions:**
    - GitHub supports numerous integrations and plugins.
    - You can automate workflows, run tests, and deploy code using GitHub Actions.

11. **Community and Social Features:**
    - GitHub encourages collaboration and interaction.
    - Users can follow each other, star repositories, and contribute to open-source projects.

12. **Gists:**
    - Gists are a way to share code snippets, notes, and small files quickly.
    - Useful for sharing code examples or collaborating on smaller tasks.

13. **Security and Code Scanning:**
    - GitHub provides security features like code scanning, dependency analysis, and vulnerability alerts.

14. **Analytics and Insights:**
    - GitHub offers insights into repository activity, including traffic, contributors, and code review statistics.

15. **Large Ecosystem:**
    - GitHub has a vast community and ecosystem.
    - It's widely adopted for open-source projects and used by many developers and organizations.

### Adding User to Git

**Global User:**  A "global user" refers to a user identity configuration that is applied to all your Git repositories on a specific system. 

- To add a global user name in your system, use the following command:
```
git config --global user.name "Your Name"
```
- To add a global user email in your system, use this command:
```
git config --global user.email "youremail@example.com"
```
**Local User:** A "local user" refers to a user identity configuration that is specific to a single Git repository.

- To add a local user name in a Git repository, use this command within the repository:
```
git config user.name "Your Name"
```
- To add a local user email in a Git repository, use this command within the repository:
```
git config user.email "youremail@example.com"
```

## Working with Remote Repository

1. **Cloning the Remote Repository**
```
git clone https://github.com/username/repository-name.git <folder_name>
```

2. **Linking the Local Repository to a Remote Repository**
```
git remote add remote_repository_name <link_of_remote_repository>
```

3. **Checking Linked Remote Repositories in Local Repository**

- To list all linked remote repository names:
```
git remote
```

- For more details, including the URLs of linked remotes:
```
git remote -v
```

4. **Removing a Linked Remote Repository from Local Repository**
```
git remote remove <remote_name>
```

5. **Updating Changes from Local Repository to a Remote Repository**
```
git push <remote_repsitory_name> <remote_repsitory_branch_name>
```

6. **Updating Changes from a Remote Repository to Local Repository**
```
git pull <remote_repsitory_name> <remote_repsitory_branch_name>
```

7. **Retrieving Changes from a Remote Repository Local Repository**
```
git fetch <remote_repository_name> <remote_repository_branch_name>:<local_branch_name>
```

### Branching
Branching is the practice of creating a separate line of development within a version control system. It allows multiple developers to work on different features, bug fixes, or experiments concurrently without interfering with each other. Each branch represents an independent path of development and can have its own set of commits and changes. Branching is used to keep the main codebase (often called the "main" or "master" branch) stable while allowing developers to work on new features or bug fixes in isolation.

1. **Creating a Branch:** A branch is a separate line of development. To create a new branch, named "feature-branch":
```
git branch feature-branch
```
2. **Switching to a Branch:** To switch to a different branch named "feature-branch":
```
git checkout feature-branch
```
3. **Pushing New Branch:** To push a new branch to the remote repository named "origin".
```
git push origin new-branch
```
4. **Pulling From a Remote Branch:** To pull from a remote repository named "origin".
```
gti pull origin branch-name
```
5. **Deleting Branch:**

- To delete the branch from local repository which has been merged to any other branch.
```
git branch -d branch_name
```
- To remove the branch from remote repository which has been deleted from local repository.
```
git push origin --delete branch_name
```

### Merging:
Merging is the process of integrating changes from one branch into another. In Git, this typically involves taking the changes made in a feature branch and applying them to the main development branch or another target branch. Merging combines the commit history and changes from one branch with another, creating a new merge commit that captures the integration of changes. Merging is used to incorporate the work done in feature branches back into the main codebase.

1. **Merge into the Main Branch:**  Once we've completed the work on our feature branch, we can merge it back into the main branch (e.g., master or main). First, switch to the main branch:
```
git checkout main
```
2. **Merge the Feature Branch:**  Then, merge our feature branch into the main branch. This will combine the changes from our feature branch with the main branch.
```
git merge feature-branch -m "Features Added"
```
**NOTE:** It will merge changes from the feature-branch only into the main branch. If you want to merge changes from the main branch into the feature-branch, you need to switch to the feature-branch and then merge from main branch.

3. **Resolve Merge Conflicts:** If there are conflicts between the two branches (i.e., both branches modified the same part of a file), Git will prompt you to resolve these conflicts manually. We'll need to edit the conflicted files, resolve the differences, and then commit the resolved files.
4. **Push Changes to the Remote Repository:** After successfully merging your feature branch into the main branch, we can push the changes to the remote repository using git push.

**A Typical Merging Workflow in Git:**
1. Create a branch for a specific task or feature.
2. Work on the branch, making commits as needed.
3. Test and ensure that your changes work as expected.
4. Merge the branch back into the main branch (e.g., main).
5. Resolve any merge conflicts, if necessary.
6. Push the changes to the remote repository.
7. Optionally, delete the feature branch after merging it to keep your repository clean.

This workflow allows multiple developers to work on different parts of a project concurrently without interfering with each other's work. It also helps maintain a clean and organized version history.


### Rebasing:
Rebasing is an alternative to merging in Git, used to integrate changes from one branch into another. Unlike merging, which creates a new merge commit, rebasing incorporates the changes by moving or replaying the commits from one branch onto another. This results in a linear commit history, making the project history appear cleaner. Rebasing is often used to maintain a more straightforward and chronological history.

1. **Rebase onto the Main Branch:** Once work on a feature branch is complete, switch to the main branch:
```
git checkout main
```
2. **Rebase the Feature Branch:** Rebase the feature branch onto the main branch. This essentially takes the changes made in the feature branch and applies them on top of the main branch:
```
git rebase feature-branch
```
3. **Resolve Rebasing Conflicts:** If there are conflicts between the two branches (i.e., both branches modified the same part of a file), Git will prompt you to resolve conflicts manually. Edit the conflicted files, resolve differences, and then continue with the rebase:
```
git rebase --continue
```
4. **Push Changes to the Remote Repository:** After successfully rebasing your feature branch onto the main branch, push the changes to the remote repository:
```
git push origin main
```

**A Typical Rebasing Workflow in Git:**
1. Create a branch for a specific task or feature.
2. Work on the branch, making commits as needed.
3. Test and ensure that your changes work as expected.
4. Rebase the branch onto the main branch to incorporate the latest changes.
5. Resolve any rebase conflicts, if necessary.
6. Push the changes to the remote repository.
7. Optionally, delete the feature branch after rebasing it to maintain a clean repository history.

Rebasing is beneficial for creating a linear and more readable history but should be used with caution in shared branches, as it rewrites commit history. It is generally recommended for feature branches that haven't been shared with others.

### Merging vs Rebasing
Both merging and rebasing are methods used in Git to integrate changes from one branch into another, but they do so in different ways, and each has its own advantages and trade-offs.

**Merge:**
- **Creates a New Commit:** When you merge branches, Git creates a new commit that has two parent commits—the latest commit from the branch you are merging into and the latest commit from the branch you are merging from.
- **Preserves the Branch History:** The branch you merged in retains its original commit history. The merge commit serves as a point where the two branches come together.
- **Easier Collaboration in Shared Branches:** Merging is generally safer in shared branches because it doesn't alter the commit history. It's a straightforward way to combine changes from multiple contributors.

**Rebase:**
- **Rewrites Commit History:** When you rebase, Git takes the commits from your branch and places them on top of the latest commit in another branch. This results in a linear history without the additional merge commit. So, force-pushing is often required after a rebase, and it should be done carefully to avoid overwriting changes on a shared branch.
- **Creates a Cleaner History:** Rebasing produces a cleaner and more linear history, as there are no merge commits cluttering the log. It makes it easier to follow the progression of changes.
- **Potential for Conflicts During Rebase:** Rebasing can introduce conflicts when applying commits on top of another branch's changes. Conflicts need to be resolved manually during the rebase process.
- **Use with Caution in Shared Branches:** Avoid rebasing if the branch has been shared with others, especially if they have already based their work on the branch. Rewriting history can cause confusion and conflicts for collaborators.

**When to Choose:**
- **Use Merge:**
   - When working on a shared branch where multiple people are collaborating.
   - To preserve a clear and accurate history of when changes were integrated.
- **Use Rebase:**
   - When working on a feature branch to keep a clean and linear commit history.
   - To integrate changes from a shared branch into your feature branch before pushing.


## Feature Branches 
Feature branches are a common practice in `Git` and `Version Control Workflows`, used to isolate and develop new features or changes in a separate branch before merging them into the `main` or `master` branch. This approach allows for more organized development, collaboration, and easier management of features and bug fixes.

- **Isolation of Work:**
  - Feature branches allow developers to work on new features, bug fixes, or enhancements in isolation. Each feature or task gets its own branch, preventing interference with the main development line or other features being developed concurrently.

- **Parallel Development:**
  - Multiple team members can work on different features simultaneously in their respective feature branches. This parallel development speeds up the overall project progress.

- **Collaboration:**
  - Feature branches facilitate collaboration by providing a dedicated space for discussion, code review, and testing related to a specific feature. Team members can collaborate on a branch and share their work effectively.

- **Testing and Quality Assurance:**
  - Feature branches serve as a staging area for testing and quality assurance. Developers can integrate and test their changes independently before merging them into the main branch, reducing the risk of introducing bugs or conflicts.

- **Code Review:**
  - Code review is more manageable with feature branches. Pull requests or merge requests can be created to review and discuss the changes made in a specific branch, enhancing code quality and consistency.

- **Version Control and History:**
  - Feature branches preserve a clear and organized version control history. Each branch's commit history reflects the development and changes associated with a specific feature or task.

- **Flexibility:**
  - If a feature or change turns out to be more complex or time-consuming than initially anticipated, the main branch remains stable and unaffected. Feature branches can be extended or adjusted as needed.

- **Rollback and Revert:**
  - If a feature branch introduces unexpected issues, it can be easily rolled back or reverted without affecting the main branch. This minimizes the risk associated with new changes.

- **Traceability:**
  - Feature branches improve traceability. You can trace back to the branch and specific commit where a particular feature was developed, which is beneficial for debugging and issue tracking.

- **Roadmapping and Planning:**
  - Feature branches can align with a project's roadmap or sprint planning. Each branch corresponds to a planned feature or task, making it easier to prioritize and execute development according to the project's goals.


## Collaborating on Git and GitHub

### Case 1: Independent Branches with Direct Push
Each Collaborator push their own branch directly to GitHub and then pull and merge to each collaborator branch to main.

**Advantages of This Workflow in a Large Team Setting**

**Parallel Development:** Developers can work independently on their own feature branches, which is advantageous for projects with a wide range of loosely related features that don't require frequent integration.

**Flexibility:** This approach offers more flexibility, allowing each developer to choose when to merge their changes into the main branch. It's useful for teams working on different timelines or with various dependencies.

**Minimal Centralization:** This approach involves less centralization, which can be beneficial for projects where strict centralization and frequent testing may not be necessary. It provides more autonomy to individual developers.

**Faster Iterations:** Developers can iterate quickly on their features without waiting for integration with a test branch, which is suitable for rapid development cycles.

**Use Case**
The 1st case, while offering advantages, comes with the trade-off of potentially less centralized testing and more individual responsibility for integration. Therefore, it's best suited for situations where a high degree of autonomy and parallel development is a priority, and the project's nature allows for less frequent integration points. Effective communication and coordination mechanisms are crucial to avoid conflicts and maintain code quality.

### Case 2: Structured Workflow with Test Branch
Main and Test branches on remote, and collaborators have their own branches only in their local repositories. They pull updates into the test branch and then merge their own branch to test and push the test branch to GitHub after a pull request is done from the test to main.

**Advantages of This Workflow in a Large Team Setting**

**Code Stability and Testing:** Maintaining code stability is crucial with a large team. This structured workflow, with a dedicated test branch, ensures that changes are integrated and thoroughly tested together, preventing unstable or untested code from entering the main branch. This aligns well with CI/CD principles.

**Isolation and Parallel Development:** Developers can work on their own feature branches independently, reducing the risk of conflicts and streamlining collaboration among a large team.

**Centralized Testing with CI/CD:** This structured approach complements CI/CD practices. Tools like Jenkins can automate testing and deployment processes. The test branch serves as a central point for automated testing, enabling continuous integration and testing of code changes—a necessity for large teams.

**Code Review:** The pull request process is essential for code review and quality assurance. In large teams, code reviews become even more critical to maintain coding standards and identify issues early.

**Traceability and Release Management:** This workflow provides clear traceability of features and bug fixes, making it easier to track their status. It also offers a predictable and controlled approach to releases, crucial for avoiding chaos during deployments in large teams.

**CI/CD Integration:** Jenkins, a powerful CI/CD tool, seamlessly integrates with this workflow. Jenkins can automatically trigger builds, tests, and deployments, enhancing development and release efficiency and reliability.

**Use Case**
The 2nd case, while offering advantages, prioritizes a more structured workflow with centralized testing and a dedicated test branch. However, this approach may entail a somewhat more intricate process. It is most suitable for projects where meticulous code stability, comprehensive testing, and efficient CI/CD practices are paramount. Given its higher degree of coordination and standardized procedures, effective communication and collaboration mechanisms remain essential to ensure smooth operations, minimize conflicts, and uphold code quality throughout the development process.


### Delete All Commit History of a Branch and Start Fresh

**Step 1:** Check Out to an Orphan Branch**
```
git checkout --orphan orphanBranch
```
**Step 2:** Add All Files
```
git add -A
```
**Step 3:** Commit the Changes to the New Orphan Branch
```
git commit -m "Initial Commit"
```
**Step 4:** Delete the Main Branch
```
git branch -D main
```
**Step 5:** Rename the Orphan Branch to the Main
```
git branch -m main