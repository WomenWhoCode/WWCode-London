# Contributing Guidelines
---


Firstly thanks for your contributions!!! :sparkling_heart::sparkling_heart:   

If you have resources you would like to share from your event or resources you think our community would benefit from keep reading!

## PRE-REQUISITE

1. 📖 Read up on fork & pull request models
2. 🍴 Fork this repo to your account
3. 🌱 Create a branch for the change you intend to make in your fork
4. ✍️ Make your changes to the above created branch in your fork
5. 🔨 Follow the contributing guidelines below
6. 🔧 Send a pull request from your fork's branch to our `main` branch
7. 🎉 Get your pull request approved - success!

## ⭐ How To Make A Pull Request:

**1.** Start by making a Fork of the [**WWCode-London**](https://github.com/WomenWhoCode/WWCode-London) repository. Click on the <a href="https://github.com/WomenWhoCode/WWCode-London/fork"><img src="https://i.imgur.com/G4z1kEe.png" height="21" width="21"></a>Fork symbol at the top right corner.

**2.** Clone your new fork of the repository in the terminal/CLI on your computer with the following command:

```bash
git clone https://github.com/<your-github-username>/WWCode-London
```

**3.** Navigate to the newly created LinkFree project directory:

```bash
cd WWCode-London
```



**4.** Create a new branch:

```bash
git checkout -b YourBranchName
```

**5.** Sync your fork or your local repository with the origin repository:

- In your forked repository, click on "Fetch upstream"
- Click "Fetch and merge"

### Alternatively, Git CLI way to Sync forked repository with origin repository:

```bash
git fetch upstream
```

```bash
git merge upstream/main
```

**6.**  ### [Github Docs](https://docs.github.com/en/github/collaborating-with-pull-requests/addressing-merge-conflicts/resolving-a-merge-conflict-on-github) for Syncing

**7.** Make your changes to the source code.

**8.** Stage your changes and commit:
```bash
git add <file/folder>
```

```bash
git commit 
```

**9.** Push your local commits to the remote repository:

```bash
git push origin YourBranchName
```

**10.** Create a [Pull Request](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request)!

**11.** **Congratulations!** You've made your first contribution to [**WWCode-London**](https://github.com/WomenWhoCode/WWCode-London/blob/main/CONTRIBUTING.md)! 🙌🏼

**_:trophy: After this, the maintainers will review the PR and will merge it if it helps move the project forward. Otherwise, it will be given constructive feedback and suggestions for the changes needed to add the PR to the codebase._**


## Adding Event Resources

1. If there is a github repository with code to share run the following in your terminal.

    ```shell
    export REPO_URL="<FILL_ME_IN>"
    cd events
    git submodule add $REPO_URL
    ```
2. Upload the event graphic to the [images](docs/images) directory if its a one-off event.
3. For programs special interest groups or programs supported by the community , Eg: machine-learning, devops, mock-behavioral-interview upload the event image under resources/[program/special-interest-group]/images

4. Copy and paste a new table entry **at the top** in the [README](README.md#event-resources). Fill in the applicable details. **Be sure to double check everything was updated.** Also be mindful of style and formatting.
<br>


    ```markdown
      <tr>
      <td style="border: none;" align="left" width="20%"><a href="$REPO_URL"><img alt="EVENT_TITLE" align="left" src="images/IMAGE_NAME"/>&nbsp;</td>
      <td colspan="3"><b>EVENT_TITLE</b>
        <br><br>
             ** EVENT_DESCRIPTION **

               <br><br>
               <em>- SPEAKER_NAME & SPEAKER_TITLE </em>

               * [Slides & Materials](SLIDE_LINK)
               * [Video Recording](VIDEO_LINK)    
               * [Slack Channel](https://wwcodelondon.slack.com/archives/SLACK_CHANNEL_ID)
      <em>- SPEAKER_NAME & SPEAKER_TITLE </em></td>
      </tr>
    ```


    <br>
    a) Image `href` should point to `$REPO_URL` from _step 1_ (this could also be a link to slides if the speaker wanted to share those without a repo.)   

    b) Image `alt` should be the `EVENT_TITLE`  

    c) Image `src` should be the relative path to the uploaded image from _step 2_   

    d) Update the `EVENT_TITLE` in the description box    

    e) Update the `EVENT_DESCRIPTION` with zoom description  

    f) Update the `SLIDE_LINK` with url to slides (if speaker has shared) and `VIDEO_LINK` with the youtube url  

    g) Update the `SPEAKER_NAME` & `SPEAKER_TITLE`  

    h) Update the `SLACK_CHANNEL_ID` from Slack workspace


## Adding New Program / Special Interest Group Resources

1. Create a new folder under `resources` with a good descriptive name for the program/ speacial interest group you are sharing.

2. Add a readme with details about the program or special interest group(what is is about, who would benefit, links, etc)

3. If sharing code, be sure to first upload the coding project to your personal repo (we want your Github profile to get all the credit). Then link to the repo by running the following in your folder from _step 1_.

    ```shell
    #make sure you are in your directory - cd DIR_NAME
    export REPO_URL="<FILL_ME_IN>"
    git submodule add $REPO_URL
    ```

## Find something to work on

The first step to getting starting contributing is to find something
to work on. Help is always welcome, and no contribution is too small!

Here are some things you can do today to get started contributing:

1. You can browse the issues labeled as [help wanted](https://github.com/WomenWhoCode/WWCode-London/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22) and [good first issue](https://github.com/WomenWhoCode/WWCode-London/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22) to see who is looking for help.

The `good first issue` label also indicates that Women Who Code - London Members have committed to providing extra assistance for new
contributors.

## Style Guide for Git Commit Messages :memo:

**How you can add more value to your contribution logs:**

- Use the present tense. (Example: "Add feature" instead of "Added feature")
- Use the imperative mood. (Example: "Move item to...", instead of "Moves item to...")
- Limit the first line (also called the Subject Line) to _50 characters or less_.
- Capitalize the Subject Line.
- Separate subject from body with a blank line.
- Do not end the subject line with a period.
- Wrap the body at _72 characters_.
- Use the body to explain the _what_, _why_, _vs_, and _how_.

## Best practices

- Write clear and meaningful git commit messages.
- If the PR will *completely* fix a specific issue, include `fixes #123` in the PR body (where 123 is the specific issue number the PR will fix. This will automatically close the issue when the PR is merged.
- Make sure you don't include `@mentions` or `fixes` keywords in your git commit messages. These should be included in the PR body instead.
- When you make a PR for small change (such as fixing a typo, style change, or grammar fix), please squash your commits so that we can maintain a cleaner git history.
- Make sure you include a clear and detailed PR description explaining the reasons for the changes, and ensuring there is sufficient information for the reviewer to understand your PR.
- Additional Readings:
    - [chris.beams.io/posts/git-commit/](https://chris.beams.io/posts/git-commit/)
    - [github.com/blog/1506-closing-issues-via-pull-requests ](https://github.com/blog/1506-closing-issues-via-pull-requests)
    - [davidwalsh.name/squash-commits-git ](https://davidwalsh.name/squash-commits-git)


## Reporting issues OR suggesting changes/features to the existing repo:

1. In order to discuss changes, you are welcome to [open an issue](https://github.com/WomenWhoCode/WWCode-London/issues) about what you would like to contribute. Enhancements are always encouraged and appreciated.
2. A repository owner will review the issue and provide feedback.
## All the best! 🥇
