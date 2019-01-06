<h1 align="center">Git Perspective</h1>

<p align="center">
<img alt="git" src="https://gitforwindows.org/img/git_logo.png" height="10%" width="10%"/>
</p>

The **Git** perspective aims at presenting a simplified interface for the most common git operations. It is built from tools that support **Git** client operations. If the user does not have any experience with **Git** then the following [link](HTTPS://rubygarage.org/blog/most-basic-git-commands-with-examples) gives a good explanation what is **Git** and the basic usage.

<p align="center">
<img alt="gitPerspective" src="./images/gitPerspective.png" height="100%" width="100%"/>
</p>

The **Git** perspective is comprised of **Git** and **Console views** and **Workspace menu**. It enables the users to perform simple git operations such as cloning a repository to a workspace, pulling changes, and pushing commits. The user can create, manage, and switch between multiple workspaces through the Workspace menu.

In order to execute a command (git operation) on a single file or folder, the user must select it and right-click to expand the menu. When executing a command, the user will be asked each time for the author name and email address to be used with the commits.
<p align="center">
<img alt="menuOnFile" src="./images/menuOnFile.png" height="50%" width="50%"/>
</p>

* The **Pull** command fetches and merges changes on the remote repository to the workspace.
<p align="center">
<img alt="gitPullOneProject" src="./images/gitPullOneProject.png" height="50%" width="50%"/>
</p>

* The **Push** command sends local commits to the remote repository. In case of merge conflict on Push operation, a new branch with the local changes will be created in the remote repository. From that point the user can use a preferred tooling to apply the actual merge between the two branches.
<p align="center">
<img alt="gitPushOneProject" src="./images/gitPushOneProject.png" height="50%" width="50%"/>
</p>

* The **Reset** command will undo the users most recent commit and put those changes back into staging, so the user does not lose any work.
<p align="center">
<img alt="gitReset" src="./images/gitReset.png" height="50%" width="50%"/>
</p>

* The **Share** command lets the user share the file or project to a specific branch in a remote repository (both branch and repository are specified).
<p align="center">
<img alt="gitShareOneProject" src="./images/gitShareOneProject.png" height="50%" width="50%"/>
</p>

In the lower menu the user has the option to perform operation on all the files in the current workspace - **Push All Projects** from the current workspace to the remote repository or **Pull All Projects** from remote repository to the current workspace. The data required to execute these commands are similar to the previous commands where only one file is effected.
<p align="center">
<img alt="pullAllProjects." src="./images/pullAllProjects.png" height="50%" width="50%"/>
</p>

<p align="center">
<img alt="pushAllProjects" src="./images/pushAllProjects.png" height="50%" width="50%"/>
</p>

The user can also clone a project with the **Clone Project** command to the current workspace.
<p align="center">
<img alt="clone" src="./images/clone.png" height="50%" width="50%"/>
</p>

<p align="center">
<img alt="gitClone" src="./images/gitClone.png" height="50%" width="50%"/>
</p>

If the user wants or needs to, he/she can easily **Refresh** the workspace.
<p align="center">
<img alt="refresh" src="./images/refresh.png" height="50%" width="50%"/>
</p>

He/She can **change workspaces** by choosing from the menu located next to the refresh button.
<p align="center">
<img alt="changeWorkspace" src="./images/changeWorkspace.png" height="50%" width="50%"/>
</p>


### References:
* Eclipse Dirigible Trial IDE links: [http://trial.dirigible.io](http://trial.dirigible.io) and [http://dirigible.eclipse.org](http://dirigible.eclipse.org)
* [http://www.dirigible.io/help/ide_perspective_git.html](http://www.dirigible.io/help/ide_perspective_git.html)

<p align="center">
<a href="http://www.dirigible.io/">
  <img src="https://github.com/eclipse/dirigible/blob/master/logo/dirigible-logo-symbol.png" width="20%" height="20% alt="dirigible logo"/>
                                                                                                                                         </a>
                                                                                                                                         </p>
