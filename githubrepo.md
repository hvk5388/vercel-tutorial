# How to create a GitHub Repostiory

GitHub is a wonderful tool for beginner programmers to learn how to use. It allows for saving code to the cloud and continuous integration. In order to use GitHub developers commit, or add, changes to code in a shared repository, or folder. This allows teams to work together and resolve issues early in the development process.

## Create Repository

**1. Open GitHub in a Browser**
Pull up GitHub [here](https://github.com/).

**2. Login or Create Account**
If you are creating an account, remember to save your password!

**3. Create a New Repo**
Once you have successfully logged in, there will be a sidebar on the left of your screen. Click on the green `new` button with the book label.
![Left Side Bar](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/tiyurg8gq0xcj7a7aolr.png)

**4. Follow the Steps to Add Basic Information**

- _Ensure `No template` is selected._ We are not using a template today, but you are welcome to experiment with this in the future.

- _Choose a repository name._ This should be unique, which the site will tell you. You can also add a description to your repository.

- _Decide public or private_. This is your personal preference.

- _Select `Add a README file`._ This includes a blank initial file in your repository.

When you are done select the green `create repository` button.
![Basic Repository Creation](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/rvqqja334wvx27pyu20r.png)

## Clone to Machine

**5. Click the Green Code Button**
At this point, your repository will have opened up. In order to get a copy on your own machine, select the green `code` button in the top right corner.
![Repository Home](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/mhcytg99n0tsl7v32tti.png)

**6. Choose the Clone Option**
Chose the copy link button under the `Clone` section in order to get the repository copied to your clipboard.
![Clone Button](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/lghro8vpelvzu755kq51.png)

**7. Open VS Code**
Using VS code, which you can download and install [here](https://code.visualstudio.com/), editing code is much easier. Terminals are included in the IDE for easy access.

**8. Select `Clone Git Repository`**
Select the clone git repository option on the hope page, under the start panel.
![VS Code Start Menu](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/8wqrru14g7aslcvt4xrr.png)

**9. Paste in the Copied link**
Paste in the link we copied from GitHub into the box that says `provide repository URL`. Select Clone from URL.

**10. Select or Create folder**
Choose where you want to locally find this code.

**11. Open Repository**
Find a way to open the new cloned repository. There may be a popup on the right corner offering to open it. If you cannot find that you may select the `Open Folder` option in the start menu.
![Open Repo Popup](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/732x4vn2lj18ofmemlws.png)

## Make Changes

**12. Find README**
Open the README file, which you should see in the left side bar. Clicking on it will open it.

**13. Edit the Code**
Add your changes to the code. The README is written in markdown. I just added a description to the repository.

```markdown
# helloworld

This is a repository for teaching GitHub basics.
```

**14. Save**
Save your changes. You can also add more folders or files in any language. GitHub can handle it all.

## Save to Github

**15. Open a Terminal**
Hover over the `Terminal` Header and select `New Terminal`.

**16. Add Changes**
Click into the terminal and type in the command `git add .`. This will save your changes.

**17. Commit Changes**
Use the command `git commit -m “added readme description”` to commit your changes with a message. You can decide what you want to write inside the quotes.

**18. Pull**
Use the `git pull` command before pushing your changes up to the GitHub. This ensure that any changes a teammate has made is in your local branch.

**19. Push**
Run the `git push` command. This will send any changes back to GitHub.

## You did it!

In order to check that your changes were saved you can head back to GitHub. You will see a time stamp and commit message on the file.
![Final Changes](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/qd569i0e1hsm9k5udbg1.png)
