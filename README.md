# How to Host a Markdown Resume Online
## Purpose
This document shows how to host a Markdown resume online using GitHub Pages. The steps will also be related to the concepts discussed in Etter's Modern Technical Writing.
## Prerequisites
To host your resume online you will need:
- Markdown Resume
- GitHub Account
  - If you do not have an account, you can make one at [github.com](https://github.com/).
- GitHub Desktop
  - If you do not have GitHub Desktop installed, instructions for installing can be found [here](https://docs.github.com/en/desktop/installing-and-authenticating-to-github-desktop/setting-up-github-desktop).

## Instructions
### Setup
1. Get your Markdown Resume.
   1. **Note:** As discussed in Etter's book we use a lightweight markup language because once learned, you can easily create formatted documents. These documents are human-readable even in the raw form and can be made using a variety of different text editors available for free. Lightweight markup can also be paired with a static site generator to easily host the document content on a website (what you are doing right now).
2. Open GitHub Desktop.
   1. **Note:** GitHub Desktop allows us to take advantage of distributed version control, in this case Git. As stated in Etter's Modern Technical Writing distributed version control allows you to make changes to your files offline. This means you can edit your resume on your computer without having to worry about messing up your online resume. It is typically used by developers to help manage changes to code but can be used to help you manage changes to your online resume as well.
3. Log into your GitHub account on GitHub Desktop.
   1. **Note:** If you need help logging in you can go [here](https://docs.github.com/en/desktop/installing-and-authenticating-to-github-desktop/authenticating-to-github-in-github-desktop).

**Result:** You should now have GitHub Desktop open and be logged in with your GitHub account.

### Create a Repository
Now you will need to create a new GitHub repository.
1. Click **File** in the top right.
2. Click **New Repository** in the drop-down.

**Result:** This should open a window to create a new repository.

3. Name the repository *username.github.io* where username is your own GitHub username.
   1. **Example:** my username is bereznyk, so I would put bereznyk.github.io
4. Click **Create repository**.

**Result:** This creates a new local repository on your computer and should set it as your current repository. Make sure that in the top right **Current repository** is set to the one you just created.

### Publish Repository
To host your resume online you will need to publish this repository to GitHub so it is online.  
1. Click **Publish repository** at the top.

**Result:** A window to publish the repository should open.

2. Uncheck the **Keep this code private** checkbox. 
   1. **Note:** In order to host your resume online the repository needs to be public.
3. Click **Publish repository**.

### Add Resume to Repository
Next, you need to add your resume to the newly created repository.
1. Click **Repository** at the top.
2. Click **Show in Explorer** in the drop-down.

**Result:** A file explorer window for your local repository should open.

3. Copy your resume into the folder on your computer.
4. Rename your Markdown resume to *index*.
   1. **Note:** The file hosted by GitHub Pages is the one called *index.md*. Make sure it has the _.md_ file extension, if your resume is named something different in the repository it will not be hosted online.

**Result:** This will add your resume to the local repository on your computer. If you go back to GitHub Desktop you should see the changes to the repository (your resume being added).

### Push to Online Repository
Now you will need to move the resume into the online repository. 
1. Click **Commit to main** in the bottom left.
   1. **Note:** A commit message is required, but you can leave it as the default chosen by GitHub Desktop. The commit message is typed in the text boxes in the bottom left box.
2. Click **Repository** at the top.
3. Click **Push** in the drop-down.

**Result:** You should see that the changes disappear in GitHub Desktop and that your resume is in the online repository. If you want to see the online repository you can click **Repository**, then **View on GitHub** at the top to open it in a web browser.

### Customize Website
Now you will customize the theme of the website for the hosted resume. To do this we will create a configuration file in the repository online. This step is not required but improves the look of your resume.
1. Click **Repository** at the top
2. Click **View on GitHub** in the drop-down.

**Result:** This should open the online repository in a web browser.

1. Click **Add File** above where your files are.
2. Click **Create new file** in the drop-down

**Result:** This should switch the page to a text editor.

5. Name the file *_config.yml* in the top left.
6. Copy the text below where it says **Enter file contents here**.
    
```yml
title: My Resume
remote_theme: pages-themes/dinky@v0.2.0
plugins:
- jekyll-remote-theme
```

7. Click **Commit changes...** in the top right.

**Result:** A window to commit the changes should pop up.

8. Click **Commit changes**.
   1.  **Note:** GitHub Pages uses a static site generator to build the page. The built-in supported static site generator for GitHub Pages is Jekyll. As stated in Etter's book a static site generator is great for easily hosting a website for your document (in this case your resume). You only need to provide the markup document and theme. If you want to change the website content you just update the markup document. These instructions provide a theme for you but in [More Resources](#more-resources) there are Jekyll and GitHub Pages resources that can help if you want to try and customize your online resume yourself.

**Note:** This will add that file only to the online repository. You can get the file into your local repository by clicking **Repository**, then **Pull** in GitHub Desktop.

### Go to Online Resume
Finally, you can go and enjoy your resume online!
1.  Go to https://username.github.io in your web browser. 
    1.  **Note:** Make sure to put your GitHub username in place of *username*.
2.  Enjoy your resume hosted online!

![](https://github.com/bereznyk/bereznyk.github.io/blob/main/resume_demo.gif)
 
## More Resources
These are some extra resources that can help you if you get stuck or want more information.
- [Markdown Tutorial](https://www.markdowntutorial.com/)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [GitHub Desktop Documentation](https://docs.github.com/desktop)
- [Git Tutorial](https://www.freecodecamp.org/news/learn-the-basics-of-git-in-under-10-minutes-da548267cc91/)
- [Jekyll Resources](https://jekyllrb.com/resources/)

## Authors and Acknowledgements
Thank you to the authors of [Dinky](https://github.com/pages-themes/dinky) for providing the theme used.

Thank you to Group 14 for helping me revise this document.

## FAQs
**Why is Markdown better than a word processor?**  
- Markdown is better than a word process because Markdown is not tied to a specific application. You can easily learn and create Markdown documents using any text editor (many of which are free). It is also widely supported, such as with static site generators.

**Why is my resume not showing up?**  
- Make sure that your GitHub repository is public and check that your Markdown resume is named "index" in the repository. Also, ensure that your resume has the ".md" file extension.


