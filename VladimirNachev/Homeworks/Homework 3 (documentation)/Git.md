# Git Perspective
## Introduction
<p>
  The Git perspective aims at presenting a simplified interface for the most common Git operations. It is built from tools that support Git client operations.
</p>
<img src="./images/startScreen.png" alt="Start screen">
<p>
  The Git perspective is comprised of Git and Console views and Workspace menu. It enables the users to perform simple Git operations such as cloning a repository to a workspace, pulling changes, and pushing commits. The user can create, manage, and switch between multiple workspaces through the Workspace menu.
  <br>
  *Note*: In case of merge conflict on Push operation, a new branch with your local changes will be created in the remote repository. From this point you can use your preferred tooling to apply the actual merge between the two branches.
</p>

## Functionalities
### 1. How to change workspace ?
<p>
  Workspaces help you to organize and manage your projects with ease.
  <br>
  You can change the workspace by opening the drop-down menu which is located at the top of the screen and selecting the wanted workspace.
</p>
<img src="./images/workspace.png" alt="Change workspace">
<p>
  In the image above there is only one workspace named **workspace**.
</p>

### 2. How to clone project ?
<p>
  You can clone project from a repository into your workspace by selecting the button <img src="./images/cloneProjectButton.png" alt="Button for cloning a project"> located at the top of the screen.
  <br>
  A view containing three fields appear on left after selecting the button.
  <br>
  <br>
  <img src="./images/cloneProjectView.png" alt="View for cloning a project">
  <br>
  <br>
  In the first field (**URL**) you should write the URL of the project that you want to clone. Second field (**Username**) is for the username and third field (**Password**) is for the password for the account in the specific implementation of the Git version control system where the project is located.
  <br>
  After you have filled in the blank fields to clone the project select the button *Clone*. To cancel the cloning procedure select the button *Cancel*.
</p>

### 3. How to pull all projects ?
<p>
  You can pull all the projects from Github (or other implementation of the Git version control system, for example Gitlab) account by selecting the button <img src="./images/pullAllProjects.png" alt="Button for pulling all projects"> located at the top of the screen and entering your credentials.
  <br>
  A view containing two fields appear on left after selecting the button.
  <br>
  <br>
  <img src="./images/pullAllProjectsView.png" alt="View for pulling all projects">
  <br>
  <br>
  First field (**Username**) is for the username and second field (**Password**) is for the password for the account in the specific implementation of the Git version control system from where you pull all projects.
  <br>
  After you have filled in the blank fields to pull all the projects select the button *Pull All*. To cancel the pulling procedure select the button *Cancel*.
</p>

### 4. How to push all projects ?
<p>
  You can push all the projects to Github (or other implementation of the Git version control system, for example Gitlab) account by selecting the button <img src="./images/pushAllProjects.png" alt="Button for pushing all projects"> located at the top of the screen.
  <br>
  A view containing four fields appear on left after selecting the button.
  <br>
  <br>
  <img src="./images/pushAllProjectsView.png" alt="View for pushing all projects">
  <br>
  <br>
  First field (**Message**) is for the commit message. Second field (**Username**) is for the username and third field (**Password**) is for the password for the account in the specific implementation of the Git version control system where you push all the projects. In the fourth field (**e-mail**) you should write your email address.
  <br>
  After you have filled in the blank fields to push all the projects select the button *Push All*. To cancel the pushing procedure select the button *Cancel*.
</p>

### 5. How to refresh the workspace ?
<p>
  You can refresh the workspace by selecting the button <img src="./images/refreshButton.png" alt="Refresh button"> located at the top of the screen.
</p>

### 6. How to pull a specific project ?
<p>
  You can pull a specific project from Git by selecting it from the workspace with right click and then choose the option *Pull* from the drop-down menu.
  <br>
  <br>
  <img src="./images/pull.png" alt="Pull option">
  <br>
  <br>
  A view appears on left which is similar to the view that appears when selecting the button <img src="./images/pullAllProjects.png" alt="Button for pulling all projects"> (*Pull All Projects* button).
  <br>
  <br>
  <img src="./images/pullView.png" alt="View for pulling a specific project">
</p>

### 7. How to push a specific project ?
<p>
  You can push a specific project to Git by selecting it from the workspace with right click and then choose the option *Push* from the drop-down menu.
  <br>
  <br>
  <img src="./images/push.png" alt="Push option">
  <br>
  <br>
  A view appears on left which is similar to the view that appears when selecting the button <img src="./images/pushAllProjects.png" alt="Button for pushing all projects"> (*Push All Projects* button).
  <br>
  <br>
  <img src="./images/pushView.png" alt="View for pushing a specific project">
</p>

### 8. How to reset a specific project from Git ?
<p>
  You can reset a specific project from Git by selecting it from the workspace with right click and then choose the option *Reset* from the drop-down menu.
  <br>
  <br>
  <img src="./images/reset.png" alt="Reset option">
  <br>
  <br>
  A view appears on left containing three fields: **Message**, **Username** and **Password**.
  <br>
  <br>
  <img src="./images/resetView.png" alt="Reset view">
</p>

### 9. How to share a specific project to Git ?
<p>
  You can share a specific project to Git by selecting it from the workspace with right click and then choose the option *Share* from the drop-down menu.
  <br>
  <br>
  <img src="./images/share.png" alt="Share option">
  <br>
  <br>
  A view appears on left containing six fields: **Repository**, **Branch**, **Message**, **Username**, **Password** and **e-mail**.
  <br>
  <br>
  <img src="./images/shareView.png" alt="Share view">
</p>

### 10. How to see underlying commands which are executed when performing a Git operation ?
<p>
  You can see what commands are used when executing a Git operation in the Console view. This can help you fix problems which arise from improper use of some of the git operations.
  <br>
  <br>
  <img src="./images/consoleView.png" alt="Console view">
</p>
