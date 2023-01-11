Session 1  - Git and Github Exercises
---

Questions have been designed to be completed in the given sequence.

1. Create a local directory on your computer named `git-workshop` and initialize it to be managed by git.

    <details>
    <summary>Solution</summary>

    ```bash
    mkdir git-workshop
    cd git-workshop
    git init
    ```
    </details>

2. Investigate the status of the repository and the branch you are currently on.
3. Rename the branch name from `master` to `main`.
4. Create a new file in `git-workshop` directory called `session1-exercise2`. Commit the file with a detailed description about the change.
5. Run commands to check the status and history of the repository.
6. Add a gitignore file to not track any log files ending with `.log` in the repository.
    <details>
    <summary>Solution</summary>
        ```bash
        touch .gitignore
        ```
        To ignore .log files we will add .log file  in .gitignore file which we created earlier.
        `*.log`
    </details>
7. Add 3 more new files called `session1-file1`, `session1-file2`, `session1-file3`. Commit each of the above file as a separate commit.
    <details>
    <summary>Solution</summary>
        ```bash
        touch session1-file1.txt
        git commit -am "Add session1-file1"
        ```
        ```bash
        touch session1-file2.txt
        git commit -am "Add session1-file2"
        ```
        ```bash
        touch session1-file3.txt
        git commit -am "Add session1-file3"
        ```
    </details>
8. Log the commit history to show only commit id and the message.
    <details>
    <summary>Solution</summary>
        ```bash
        git log --oneline
        ```
    </details>

9. Edit the last commit message in `main` to `edit commit message for exercise7`
    <details>
    <summary>Solution</summary>
        ```bash
        git switch main
        git commit --amend -m "Update commit for session1-file3"
        ``` 
    </details>
10. Investigate where the `HEAD` is pointing to.
11. Investigate all existing branches. Create a new branch `session1` and switch to it.
12. Investigate all existing branches and `HEAD` now.
13. Add a new file `random` in `session1` branch and commit the changes. Investigate `HEAD`.
14. Create a new branch `feature1` from the branch `session1`. Switch to branch `feature1`. Investigate all existing branches and `HEAD` now.
15. Delete `feature1` branch.
16. Switch to `main`. Edit the file `session1-file1` in the `main` branch and add the name of the branch "MASTER" in the file. Stage and commit the changes made to the file.
17. Switch to the `session1` branch, and edit the same file `session1-file1` in the session1 branch and add the name of the branch "SESSION1" in the file.
18. Your changes in the `session1` branch is in the draft stage (not staged or committed). Now try to switch back to the `main` branch. Resolve the issue reported by git without committing your draft changes and switch to `main`.
19. Now switch back to `session1` branch (assume your changes are now finalized). Commit the changes that were in the draft stage (ie: the file `session1-file1` with the name of the branch "SESSION1" in it).