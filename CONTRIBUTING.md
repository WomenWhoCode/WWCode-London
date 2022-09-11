# Contributing Guidelines
---


Firstly thanks for your contributions!!! :sparkling_heart::sparkling_heart:   

If you have resources you would like to share from your event or resources you think our community would benefit from keep reading!

## Pre-Reqs

1. 📖 Read up on fork & pull request models
2. 🍴 Fork this repo to your account
3. 🌱 Create a branch for the change you intend to make
4. ✍️ Make your changes to the above created branch in your fork
5. 🔨 Follow the contributing guidelines below
6. 🔧 Send a pull request from your fork's branch to our `main` branch
7. 🎉 Get your pull request approved - success!

## Adding Event Resources

1. If there is a github repository with code to share run the following in your terminal.

    ```shell
    export REPO_URL="<FILL_ME_IN>"
    cd events
    git submodule add $REPO_URL
    ```
2. Upload the event graphic to the [images](docs/images) directory.

3. Copy and paste a new table entry **at the top** in the [README](README.md#event-resources). Fill in the applicable details. **Be sure to double check everything was updated.** Also be mindful of style and formatting. 
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
         </td>
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
    
    h) Update the SLACK_CHANNEL_ID from Slack worspace



## Adding Other Resources

1. Create a new folder with a good descriptive name for the resources you are sharing.

2. Add a readme with details about what is being shared (description, links, etc)

3. If sharing code, be sure to first upload the coding project to your personal repo (we want your Github profile to get all the credit). Then link to the repo by running the following in your folder from _step 1_.

    ```shell
    #make sure you are in your directory - cd DIR_NAME
    export REPO_URL="<FILL_ME_IN>"
    git submodule add $REPO_URL
    ```

## How to write a Git Commit Message

Please read [this](https://cbea.ms/git-commit/) article on best practices to writing a git commit message and follow guidelines for commiting changes to this repo. 