<img style="display: none;" src="https://static.bc-edx.com/ai/ail-v-1-0/prework/m2/img/banner.jpg" alt="lesson banner" />

Now that you've installed your tools for the boot camp, we need to set up a few things so that we can get the most out of VS Code.

Carefully follow the instructions, step by step. As developers, an essential skill is understanding and interpreting documentation.

You will need to open VS Code to proceed.

## Edit Settings

### Set Up Rulers

The recommended character limit for lines of code in Python is 79 characters. We don't want to have to count characters ourselves to ensure we're not going over that limit, so we can change our settings to display a ruler when we open our files. To do this, proceed with the following steps.

1. Click on the settings button in the lower right corner of the window that looks like a gear, then click "Settings". If you can't find the icon, you can also go into the "Code" menu, then "Settings...", then click "Settings". Alternatively, you can use keyboard shortcuts: `Ctrl+,` on Windows or `Cmd+,` on a Mac.

2. In the search bar, type "ruler." Scroll down to the "Editor: Rulers" setting and click "Edit in settings.json"

3. You will find some text that looks something like the following:

    ```json
    {
        "editor.rulers": [

        ]
    }
    ```

    You will want to edit the `"editor.rulers"` setting so that it has the number 80 inside the square brackets, like so:

    ```json
    {
        "editor.rulers": [
            80
        ]
    }
    ```

4. Save and close this file.

### Set Up Shell Command (Mac only)

If you're a Windows user, you can skip this step, as this command comes preinstalled. Instructions to use the shell command will follow.

1. In VS Code, select View in the menu.

2. Select the first option, Command Palette.

3. Type "shell" and select "Shell Command: Install 'code' command in PATH/”

## Accessing VS Code from the Command Line Interface

When you have installed VS Code, you can open it via the command line interface (CLI). You can access the command line by opening Terminal on macOS or using Git Bash on Windows. This is a useful way to automatically open so that all files in a particular directory are accessible from the Explorer menu in VS Code. You will learn how to navigate to specific directories from the CLI during your first week of class.

To test opening VS Code from the command line before class starts, do the following:

1. Open Terminal on macOS or Git Bash on Windows.

2. Type `code .` to open VS Code.

> **Note:**
>
> For Windows users, this command is already installed and ready for use, but you must restart your CLI console for the command to work.
>
> For macOS users, you will need to follow the steps to set up the shell command before this will work.
