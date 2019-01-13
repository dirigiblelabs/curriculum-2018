# Eclipse Dirigible - Git Perspective

Eclipse Dirigible is an Integrated Development Environment as a Service (IDEaaS) for dynamic applications. It provides both development tools and runtime environment. The IDE contains different perspectives which simplify the user interaction with the IDE itself and the outher services such as GitHub, GitLab, BitBucket.
The Git perspective aims at presenting a simplified interface for the most common git operations. It is built from tools that support Git client operations. It enables the users to perform simple git operations such as cloning a repository to a workspace, pulling changes, and pushing commits. The user can create, manage, and switch between multiple workspaces through the Workspace menu.

## The Git perspective is comprised of:

  - Git
  - Workspace menu
  - Console views

### Git
Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency. 
Before we start work with git we have to have already created repository where to commit our Dirirgible project or to create one.
![git_repo_create.png](https://www.dropbox.com/s/6s7gc3yo1psxyzo/git_repo_create.png?dl=0&raw=1)
After that we need the url of that repository because we will use it later. The URL is necessary to share the Eclipse Dirigible project with the GitHub repository.
![repo_url.png](https://www.dropbox.com/s/sncyhf4hmytuj0p/repo_url.png?dl=0&raw=1) 

### Workspace menu
The Workspace is the developer’s place where he/she creates and manages the application artifacts. The first-level citizens of the workspace are the projects. Each project can contain multiple folders and files (artifacts). The workspace menu is part of the workspace. It takes place at the left part of the IDE's window. 
We have to create a new Dirigible project first.
![create_project.png](https://www.dropbox.com/s/v4ziys1stqkar8j/create_project.png?dl=0&raw=1)
Next genereate HelloWorld file. We are going to use a Hello World JavaScript template for demonstration purpose.
![generate_file.png](https://www.dropbox.com/s/vg0zew2zj26yo9k/generate_file.png?dl=0&raw=1)

Now we have simple and small working project. Now let's share the Dirigible project with the priviously created GitHub repository. For this purpose from the Workspace menu we have to choose the Git icon. This actually is simplified Git interface from where easily user can push, pull, reset or share his Dirirgible project.
![proj_git.png](https://www.dropbox.com/s/qv8uvnjmp25kswd/proj_git.png?dl=0&raw=1)

If we commit for the first time then we have to choose the Share option and fill the form with our git credentials and git repository and the branch name.
![git_share.png](https://www.dropbox.com/s/de0xgv6oiqaf706/git_share.png?dl=0&raw=1)

Go back to your GitHub account. As you can see, the project has been shared successfully.

![git.png](https://www.dropbox.com/s/qir2o273mbziigl/git.png?dl=0&raw=1)

Once we have deployed our project we can push or pull changes. 

### Console view
![console.png](https://www.dropbox.com/s/6v7ewkjvg7je4s5/console.png?dl=0&raw=1)
The console takes part in git section of workspace menu. It is readonly and gives us an information about actions related to git such as errors, infos, warnings, date and hour of the information. From the console we can figure out if everything works well and we can get some feedback about our actions.

