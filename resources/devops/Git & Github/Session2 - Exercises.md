Session 2  - Git and Github Exercises
---

Questions have been designed to be completed in the given sequence and is a continuation of exercises in [Session 1](Session1%20-%20Exercises.md). All the files in the exercises refer to `.txt` files.

1. Change directory to `git-workshop` and investigate the existing branches, commit history and status.

    <details>
    <summary>Solution</summary>

    ```bash
    cd git-workshop
    git branch
    git log
    git status
    ```
    </details>

2. Create a new branch `session2` from the `session1` branch. Switch to the `session2` branch. Investigate where the HEAD is pointing to.
3. Add a new file `session2-file1` in the `session2` branch. Commit this new file to your local repository.
4. Edit the file `session2-file1` and add "SESSION2-RESTORE-STAGING" to the file. Add these changes to the staging area (do not commit the changes at this stage). Check the status of your local repository.
5. Unstage the changes in the file `session2-file1`. Check the status of your local repository.
6. Undo the changes in the file `session2-file1` and restore the file to HEAD. Check the status of your local repository. Make sure that there are no changes to be committed.
7. Create 8 new commits in the branch `session2`. These can be any random commits that you can track easily. For simplicity you can use the format that was used during the session 2 event - Enter numerical values (ONE, TWO, THREE, etc) in the file `session2-file1` and commit after adding each value. Use commit messages that are easier to track ( Commit 1, Commit 2, Commit 3, etc). Check the commit history.
8. Undo the last 2 commits from the local repository such that the changes made are preserved in the working directory. Check git history and status. Undo the changes that exist in the working directory. You should see 6 new commits in the log at this stage
9. Undo the latest 2 commits without preserving any changes made in these commits to the local directory. You should only see 4 new commits in the log at this stage.
10. Undo the latest 2 commits by preserving the git history that these commits were made and reverted.