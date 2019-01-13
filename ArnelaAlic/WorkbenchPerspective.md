# **Workbench Perspective**

This is the place where the user develops the dynamic applications. This perspective contains all views and editors that may help in the overall implementation, from domain models via services to the user interface.

![](https://i.imgur.com/7SLJrw1.png)

The Workbench consists of the following functionalities:

* _**Workspace:**_

One of the first things you specify when you start Eclipse is the workspace location. The workspace is a directory that holds information about the projects you work on, as well as the Eclipse preferences (from layout to behavior). We can say that the workspace "holds" the Integrated Development Environment: the data you work on (organized in projects) and how you work with it (preferences). It is your "space of work" or "working space" or "working universe".

The projects (your data) are not necessarily physically located in the workspace directory. They can be simple pointers to other locations on the disk. However the workspace aggregates all your "relevant" projects for a specific development universe.

![](https://i.imgur.com/DkD9wLb.png)

When you create a new empty project in the workspace, it is located in the actual workspace directory. When you create a project from existing source, the workspace keeps a pointer to the project folder. When you import a project in your workspace, again the workspace keeps a pointer to the project folder. (Importing is an interesting concept, documented separately).


* _**Import:**_

The Import view enables the user to upload a *.zip file, containing one or more projects, to the selected Workspace. The view includes a progress bar for navigation of the process. The user can manage and switch between multiple workspaces through the Workspace menu.

![](https://i.imgur.com/mLXquZI.png)


* _**Properties:**_

When you choose a file, or folder in your workspace you can see its properties in the section _"Properties"_. Each file/folder has the following properties:

_1. name_

_2. path_

_3. type_

_4. contentType_

_5. label _

![](https://i.imgur.com/S1H9cy3.png)

* _**Preview:**_

The _"Preview"_ section displays the result of executing the selected file. When you save the changes it refreshes automatically. If it is needed the user can refresh it manually by clicking the refreshing symbol (⟳).

![](https://i.imgur.com/tFaubf7.png)

* _**Console:**_

Console object is used to write messages to the default logging output. It has several log levels INFO, WARNING, ERROR, TRACE. 
The console plays a debugger role for the user, indicating where there is _"INFO, WARNING, ERROR, TRACE"_. 

![](https://i.imgur.com/nBRS3qv.png)