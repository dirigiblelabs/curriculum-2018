#
# Workbench Perspective

This is the place where the user develops the dynamic applications. This perspective contains all views and editors that may help in the overall implementation, from domain models via services to the user interface.

![](https://github.com/dirigiblelabs/curriculum-2018/blob/master/StoyanTomitsin/ide_workbench_perspective.png)

The Workbench perspective is comprised of Workspace, Import, Properties, Console and Preview views, plus the editors registered for each file type. In other words, the minimal toolset for file management, preview and editing operations.

The main view opened by default in this perspective is:

- _Workspace_ explorer (a standard view on the projects in your workspace)

## Views

- **Workspace view**

The  **Workspace**  is the developer&#39;s place where he/she creates and manages the application artefacts. The first-level citizens of the _workspace_ are the _projects_. Version 3 of Dirigible enables the users to create, manage, and switch between multiple workspaces through the Workspace view. Each project can contain multiple folders and files (artefacts). The new template-based project and artefacts scaffolding generators features are worthy of mention. The projects file organization is now non-normative and entirely up-to the preferences of the users. The IDE supports multiple editors registered for different file (MIME) types. More than one editor can be registered for one file type and in this case a &quot;Open with…&quot; context menu entry is rendered for the user to select, which one to use. The Workspace explorer displays a standard view on the projects in your workspace. It shows the folder structure along with the files.

![](https://github.com/dirigiblelabs/curriculum-2018/blob/master/StoyanTomitsin/ide_view_workspace.png)

There is a context menu assigned to the project node:

![](https://github.com/dirigiblelabs/curriculum-2018/blob/master/StoyanTomitsin/ide_workspace_menu_new.png)

Via this context menu, you can create new artefacts such as:

-
  - Database Table
  - Database View
  - Database Schema Model
  - Entity Data Model
  - JavaScript Service
  - HTML5 Page
  - Scheduled Job
  - Message Listener
  - Business Process Model
  - Access Constraints
  - Roles Definitions

or just regular ones:

-
  - File
  - Folder



- **Import view**

![](https://github.com/dirigiblelabs/curriculum-2018/blob/master/StoyanTomitsin/ide_view_import.png)

The Import view enables the user to upload a \*.zip file, containing one or more projects, to the selected Workspace. The view includes a progress bar for navigation of the process. The user can manage and switch between multiple workspaces through the Workspace menu.

- **Console view**

The Console view is a major debugging tool. It displays the output of the code that you are executing.

![](https://github.com/dirigiblelabs/curriculum-2018/blob/master/StoyanTomitsin/ide_view_console.png)

- **Preview view**

The Preview view displays the result of executing the selected file. It refreshes automatically during Workspace change events e.g. Save.

![](https://github.com/dirigiblelabs/curriculum-2018/blob/master/StoyanTomitsin/ide_view_preview.png)

**References:**

- [http://www.dirigible.io/help/ide\_perspective\_workbench.html](http://www.dirigible.io/help/ide_perspective_workbench.html)
- [http://www.dirigible.io/help/index.html](http://www.dirigible.io/help/index.html)
- [http://trial.dirigible.io](http://trial.dirigible.io)
