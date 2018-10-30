# ECLIPSE DIRIGIBLE



- **What&#39;s Eclipse Dirigible?**

Eclipse Dirigible is online, cloud development platform. The platform provides different tools, used for developing.It provides online runtime environment.

- **Motivation for usage**

Dirigible supports full development life-cycle of on-demand applications, programming models and rapid application development techniques. The platform provides all capabilities for developing process through RESTfull services authoring, patern-based user interface, testing, debugging, operations, monitoring and many other functions. Dirigible platform is completely free – all project&#39;s source code and applications are licensed and maintained at GitHub. You can use it despite your age, supervisors and job. It has different sections for education, developers and even business, different tutorials, blogs and forum, where you can ask questions and find information. Dirigible is all you want of a cloud development platform.

- **What you may do in Dirigible as a programmer – simple example.**

You want an application that tells you whose namedays are coming next in the recent days, according to people, registered for it.

- **How to do that?**

1. Go into the Dirigible Web IDE.  Create new project and name it. Choose the blank template.
2. To create data structure, select_New_ _-\&gt;_ _Data structure._
3. Choose relational database table with 3 columns - id, name, age. Create them with the **Add**
4. For the first column fill: name -_ID_, type -_Integer_ and check the boxes _Not null?_ and _Primary key._

For the second one fill:name - _NAME_, type – _VARCHAR_, length -_255,_ checkbox _Not null?._

For the last column fill:  name -_AGE_, type _–_ _Integer__,_ checkbox _Not null?._

1. Name the table, format
2. To generate a scriptings service providing CRUD database operations, select the project, _New_ _-\&gt;_ _ScriptingService_.
3. In the template window select_JavaScript Entity Service__._
4. On the next page select the table you have created.Name the service.

As a result, in the workspace explorer, under ScriptingServices, Eclipse Dirigible generated for you an entity based on the table, a RESTfull, a swagger API documentation and a library providing CRUD database operations.

1. T create an application, people are going to use to register for the nameday, select the entity, Generate _-\&gt;_ _User Interfacee for Entity Service_.
2. Choose_Mobile Create Entities_ template.
3. Select the fields to be visible during registration and change the text of the labels that are dispplayed.
4. Load the application form and put it under the package register.
5. Give the application a T be more personalized, change the message, n line 80 of the code, that displayed when a person successfully creates a new entity.
6. To create a separate application to view people who registered for the nameday, select the entity, _Generate_ _-\&gt;_ _User Interface for Entity Service_.
7. Choose_the Mobile List and Manage Entities_ and the columns to be visible.
8. Name the main file and put it under the package manage. Then give the application a title.

As a result, Eclipse Dirigible generated for you another application under the _MobileApplications_ directory, which is enerated under the manage package.