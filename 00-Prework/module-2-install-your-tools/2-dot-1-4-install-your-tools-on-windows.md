<img style="display: none;" src="https://static.bc-edx.com/ai/ail-v-1-0/prework/m2/img/banner.jpg" alt="lesson banner" />

Now it's time to collect your tools and begin. This page contains the setup guides for Windows. If you are on a Mac and have already completed the installs on the previous page, click Next to skip this page. Follow the instructions closely and do your best with the information you have—we know there's a lot to install!

### Before You Begin

First, create accounts for the following services, which you'll need throughout the course. Don't just create logins; job recruiters often scour these sites in search of job candidates, so be sure to provide at least a headshot and contact information.

*   [LinkedIn](https://www.linkedin.com/)

> **note**
>
> You should create a full profile highlighting your skills and work experience, and include a headshot.

*   [GitHub](https://github.com/)
*   [Stack Overflow](http://stackoverflow.com/)

In addition, be sure to accept the invite for your section on [Slack](https://slack.com/). You will receive the link to your class-specific channel near the start of your first class.

## Tool and Software Installations

Follow these instructions to complete the installation process for all of the required tools.

## Google Chrome

1.  If you don’t already have Chrome installed, visit the [download page](https://www.google.com/chrome/browser/desktop/index.html).
2.  Download, open, and run the installation file.

## Slack

1.  Go to [Slack for Windows](https://slack.com/downloads). Click **Download**.

2.  When the installation is complete, add our channel to your application.

3.  Click the header of your current Slack channel.

4.  Select "Sign in to another team."

5.  Enter the Slack domain provided to you near the start of your first class.

    ![A screenshot shows the Slack interface.](https://static.bc-edx.com/ai/ail-v-1-0/prework/m2/img/Install-Slack3.1.jpg)

6.  Enter your email (the one that the Slack invite was sent to) and password.

## Git and Git Bash

1.  Go to the Git [Downloads](https://git-scm.com/downloads) page. Select the download for Windows. It should automatically download the most up to date version, which is totally fine!

2.  Select Next to progress through the installation until you get to the screen that asks you to choose a default editor for Git. Select "Use Visual Studio Code as Git's default editor."

    ![A screenshot shows the Git installation screen for Windows.](https://static.bc-edx.com/ai/ail-v-1-0/prework/m2/img/git-vs-code-screen.jpg)

3.  When you are prompted to answer "How should Git treat the line endings in text files?", select "Checkout as-is, commit Unix-style line endings. Then, select next.

    ![A screenshot shows the prompt screen for Windows.](https://static.bc-edx.com/ai/ail-v-1-0/prework/m2/img/Install-GitWindows2.3.jpg)

4.  Select "Use Windows' default console window."

    ![A screenshot shows the Git installation prompt for Windows.](https://static.bc-edx.com/ai/ail-v-1-0/prework/m2/img/Install-GitWindows2.4.jpg)

Any settings not mentioned here can be left in their default mode.

## GitHub Token Setup Guide

To complete the following steps, you'll need to sign up for an account on the [GitHub website](https://github.com/) if you haven't already.

1.  Click your profile image in the top-right corner of the GitHub website, and choose Settings from the dropdown menu.

    ![A screenshot showing the profile menu with the Settings option](https://static.bc-edx.com/ai/ail-v-1-0/prework/m2/img/profile-then-settings.jpg)

2.  Scroll down and select "Developer settings" on the left, as shown in the following image:

    ![A screenshot displays various options under the Settings menu, including Developer settings.](https://static.bc-edx.com/ai/ail-v-1-0/prework/m2/img/tokensetup-developer-settings.jpg)

3.  Then click "Personal access tokens" from the left, as shown in the following image:

    ![A screenshot shows the Personal access tokens option under GitHub Apps.](https://static.bc-edx.com/ai/ail-v-1-0/prework/m2/img/tokensetup-personal-access-tokens.jpg)

4.  Click "Generate new token" in the upper right, configure for "No expiration," and check the "repo" box for full control of private repositories, to match the following image:

    ![A screenshot displays the New personal access token page, with the no expiration and repo options selected.](https://static.bc-edx.com/ai/ail-v-1-0/prework/m2/img/tokensetup-new-personal-access-token.jpg)

5.  After generating the token, leave the page open. You will need to use the token for authentication in a later step.

Next, follow these steps in your command line:

1.  Enter the following code with your GitHub username, then hit Enter to set your git username.

`git config --global user.name <your_username>`

2.  Next, enter `git config --global user.password <your_token>` using your personal access token from the GitHub window left open in the previous step in place of a password, then hit Enter.

Nice work! You have now completed the Token Setup. As you will learn, GitHub is a collaborative tool—you can pull any changes down to your local repository quickly and easily, allowing you to easily share different versions of your code across workstations and to easily checkout and test those versions on your local computer.

## VS Code

1.  Go to the [setup page](https://code.visualstudio.com/docs/setup/setup-overview) on the VS Code website and select Windows as your platform.
2.  When the download is complete, run the installer file (VSCodeSetup-version.exe).

> **note**
>
> For a 64-bit machine, VS Code is installed under `C:\Program Files \(x86\)\Microsoft VS Code`.

Great work on your Windows installations!
