# Visual Studio Code and GitHub integration
Step-by-step instructions on how to use Visual Studio Code to create, clone or edit GitHub repositories.

# Pre-requisites
On your own computer, you need to have the following installed:
- [Git](https://git-scm.com/downloads) (close Visual Studio Code and reopen after installing)
- [Visual Studio Code](https://code.visualstudio.com/)

On university machines, open [AppsAnywhere](https://appsanywhere.port.ac.uk/), search for and install the following in this order:
- "Git"
- "Visual Studio Code"

## Test your installation
Open a terminal (or command prompt on Windows) and type the following:
```bash
git --version
```
You should also configure your name and email address for Git:
```bash
git config --global user.name "Your Name"
git config --global user.email "Your Email"
```
Replace `"Your Name"` with your GitHub username and `"Your Email"` with the email address you used to create your GitHub account.

# Create a new repository
- In Visual Studio Code, open the command palette (Ctrl+Shift+P or Cmd+Shift+P on Mac) and type `File: Open Folder` to open a folder containing your existing code or a new folder.
- Open the command palette again and type `View: Toggle Source Control` to open the Source Control panel.
- Click on the `Publish to GitHub` button.
- In the opened entry field, type the name of your new repository, choose between `Public` and `Private` and click `Enter`.
- You may be asked to choose which files/folders to include in the repository.      
    - On Python projects uncheck the `env` and `__pycache__` folder.
    - On a `Node.js` project uncheck the `node_modules` folder.
- You may be asked to sign in to GitHub. If so, follow the instructions on screen.
- Once successful, you should see a message in the bottom right corner of the screen saying `Successfully published "Your Repository Name" to GitHub`. Click on the `Open` button to open the repository in your browser.

# Clone an existing repository
- In your browser, open the repository you want to clone and copy the URL from the address bar.
- In Visual Studio Code, open the command palette (Ctrl+Shift+P or Cmd+Shift+P on Mac) and type `Git: Clone` to open the Clone Repository panel. Then paste the URL you copied from GitHub and press `Enter`.
- Choose a folder on your computer where you want to clone the repository and press `Enter`.
- You may be asked to sign in to GitHub. If so, follow the instructions on screen.
- Once successful, you will be asked to open the repository on the current or new window.

# Edit an existing repository
- Follow [Clone an existing repository](#clone-an-existing-repository) instructions to clone the repository or [Create a new repository](#create-a-new-repository) instructions to create a new repository.
- Open the folder containing the repository in Visual Studio Code.
- Make changes to the files in the repository (for example, add a new file or edit an existing file). Save your changes with `Ctrl+S` or `Cmd+S` on Mac.
- You should see a number next to the `Source Control` icon in the left panel. Open the command palette (Ctrl+Shift+P or Cmd+Shift+P on Mac) and type `View: Toggle Source Control` to open the Source Control panel.
- You should see a list of files that have been changed. Click on the `+` icon next to a changed file to stage it for commit.
- Type a commit message in the text box at the top of the panel that describes the changes you made and press `Ctrl+Enter` or `Cmd+Enter` on Mac to commit the changes.
- A new button should appear at the top of the panel saying `Sync Changes`. Click on it to push your changes to GitHub.
- To confirm that your changes have been pushed to GitHub, open the repository in your browser and check that the changes are there.
- To "pull" changes from GitHub to your local repository, open the command palette (Ctrl+Shift+P or Cmd+Shift+P on Mac) and type `Git: Pull` to pull the changes from GitHub to your local repository. You could also do the same by clicking on the `Synchronize `Changes` button on the left side of the status bar at the bottom of the screen.