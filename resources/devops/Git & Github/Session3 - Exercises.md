Session 3  - Git and Github Exercises
---

Questions have been designed to be completed in the given sequence and is a continuation of exercises in [Session 2](Session2%20-%20Exercises.md). All the files in the exercises refer to `.txt` files.

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

2. Set up Two factor Authentication on your github account.
3. Set up SSH key for your github account.
4. Host the local repository `git-workshop` that you have been working on to your github account.
5. Create a new branch `session3` from the `session2` branch. Switch to the `session3` branch. Add a new file `session3-file1` in the `session3` branch. Push these changes to the remote github repository.
6. Investigate remote fetch and push urls, local and remote branches for the `git-workshop` repository. Configure the local repository to push to the configured remote repository by just using the `git push` command.
7. Create a new github repository called `wwc-london-github-workshop`. Clone the repository to your local system. Investigate remote fetch and push urls, local and remote branches, status of your local repository.
8. Create a new branch called `session3` in the remote repo from the `main` branch. Check if the `session3` branch is available in your local repo. Switch to the `session3` branch in your local repo.
9. With `HEAD` pointing to `session3` branch create a file called `members`, add your name and current location to it. Check the status of the repository now. Check if you changes are now available on the github repository. Make your changes available to the remote github repository.
10. Emulate new changes have occurred in the remote repository `wwc-london-github-workshop` by adding a new line directly via github to the `members` file which includes the name and location of another fellow WWC-London member.
11. Check if these changes are available in local repository. Run appropriate command so that your local repository has information about changes in the remote repository (without applying the changes to your local repository) Check the status and logs. Check if the file `members` has been updated.
12. Run appropriate command to get these changes from the remote github repository to your local repository. Check the status and logs. Check that the file `members` has the changes.
