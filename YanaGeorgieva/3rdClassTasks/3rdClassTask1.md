# Eclipse Dirigible™

## Basic Information

**Eclipse Dirigible**  is an Integrated Development Environment as a Service (IDEaaS) for dynamic applications. It provides both development tools and runtime environment.

<p align="center">
  <img src="https://github.com/eclipse/dirigible/blob/master/logo/dirigible-logo-symbol.png" width="60%" alt="dirigible logo"/>
</p>

### Enjoy Programming Like Never Before

From the end user&#39;s perspective (developer), Dirigible runs directly in the browser, therefore does not require any downloads or installations.

From the service provider&#39;s perspective (PaaS/SaaS), Dirigible packs all required components in a self-contained software bundle that can be deployed in any Java-based web server, such as Tomcat, Jetty, JBoss.

Dirigible supports access to RDBMS via JDBC. Currently supported versions for RDBMS are HANA, MaxDB, Sybase ASE, PostgreSQL, MySQL, H2, and Derby.

Dirigible promotes the In-System Programing development model, where you make dynamic alteration of the live system. To provide the self-contained bundle serving all the needed features for a business application, Dirigible packs various engines such as ActiveMQ, Quartz, Lucene, Flowable, Mylyn, Rhino, V8 and others.

The project started as an internal SAP initiative to address the extension and adaption use-cases related to SOA and Enterprise Services.

## Motivation to use the platform

Nowadays, providing a full-stack application development platform is not enough. Building and running on top of it has to be fast and smooth! Having that in mind, slow and cumbersome _&quot;Build&quot;_, _&quot;CI&quot;_, and _&quot;Deployment&quot;_processes have a direct impact on development productivity. In this line of thought, it isn&#39;t hard to imagine that the Java development model for web applications doesn&#39;t fit in the cloud world. Luckily, one of the strongest advantages of Dirigible comes at hand - the  **In-System Development**  model. Right from the early days of Dirigible, it was clear that it is going to be the platform for  **Business Applications Development**  in the cloud and not just another general purpose IDE in the browser. The reason for that decision is pretty simple - _ **&quot;One size doesn&#39;t fit all&quot;** _! Making a choice between providing &quot;In-System Development&quot; in the cloud and adding support for a new language _(Java, C#, PHP, …)_, is really easy. The new language doesn&#39;t really add much to the uniqueness and usability of the platform, as the In-System development model does!

## A step by step example of how to create native mobile applications with Eclipse Dirigible and Tabris.js

Here is a youtube video tutorial and a guide written step by step what to do: 

<a href="http://www.youtube.com/watch?feature=player_embedded&v=0a1t2BsO8XA
" target="_blank"><img src="http://img.youtube.com/vi/0a1t2BsO8XA/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>

### Steps:

1. We go into the Eclipse Dirigible Web IDE. We&#39;ll start off by creating an empty project.
2. We click on New in the workspace explorer on the left and from the dropdown menu select Project.
3. In the new project wizard we give our project the name &quot;nameday&quot; as that&#39;s what we&#39;re going to use it for. Click next.
4. We can select one of the predefined project templates, but as we won&#39;t be needing that, we select Black application and click Finish.
5. In the left under the workspace explorer you see the basic structure of one Eclipse Dirigible Project. You have the DataStructures, MobileApplications, ScriptingServices and so on.
6. Right click on the project and under New select Data Structure.
7. We want to crate a Relational Database Table so we select it and click next.
8. The first column of the table will be the id: Click add to add a new column. For the column name type ID, give it an INTEGER type and check the not null and primary key boxes. The second column is the name of the person who&#39;s going to register for the party. Again, click Add and for the column name type NAME, select VARCHAR type and set it&#39;s length to 255. This time select only the not null checkbox. The last column we want to add is the age. Click Add and for name type AGE, select INTEGER type and again select the not null checkbox.
9. Give the table a name – we&#39;ll call it nameday.table
10. Now you see in the workspace explorer under DataStructures we have our table defined and in the editor in the right you can see it&#39;s definition in JSON format.
11. For this data structure we want to generate a scripting service providing CRUD database operations. For this purpose, right click on the project and under New select ScriptingService. From the available templates select JavaScript Entity Service on Table. On the next page we select our table that we created. It&#39;s called nameday. Give the service a name – we&#39;ll call it nameday.js and click finish.
12. As you can see in the workspace explorer, under ScriptingServices Eclipse Dirigible generated for us an entity based on the table, a RESTfull on the endpoint nameday.js, a swagger API documentation and a library providing CRUD database operations.
13. Okay, now we want to create the application, people are going to use to register for the nameday. Right click on the entity and under Generate select User Interface for Entity Service. From the predefined templates select Mobile Create Entities as this is the most appropriate template for our case where we want to register people. Click next and we have all the fields defined for this entity. We select the ones we want to be visible during registration and change the text of the labels that are displayed. For name we&#39;ll put &quot;Your name&quot; and for age – &quot;Your age&quot;. Click next. Now we specify the main file that tabris.js is going to load our application from. We&#39;ll give it the name register.js and we&#39;ll put in under the package register. Click next and give the application the title &quot;Register for nameday&quot;. Click on finish and now under MobileApplications in the workspace explorer we have the package register and a basic tabris.js project created for us. Now for this to be more personalized we&#39;ll open the register.js file and change the message displayed when successfully created a new entity. On line 80 change the text to &quot;You have successfully registered for the nameday&quot; and click save.
14. I want a separate application in which I can view who&#39;s registered for the nameday. Again, right click on the nameday entity and under Generate select User Interface for Entity Service. Now from the predefined templates select Mobile List and Manage Entities. Select the columns that I want to view, click next and give the main file the name &quot;manage.js&quot; and put in under the package manage. Click next and give the application the title &quot;View who&#39;s coming&quot;. When we select Finish, we have another application generated for us under the MobileApplications directory. This one is generated under the manage package.
15. Now we take out our phones, open Tabris.js and go to the URL tab. Enter the URL that I&#39;ve typed here (MAKE SHORT-URL FOR REGISTRATION AND MANAGEMENT) and click Connect. You&#39;re prompted with the registration application. As you can see the labels and the title are the ones we&#39;ve put. We&#39;ll register a fake user with the name George and we&#39;ll set his age to be 23. Click Save and as you can see we have the confirmation message we put a while ago.
16. Swipe from the right to the left end of the screen, click on the home icon and this time go into the manage application. Now in the URL we substitute &#39;register&#39; with &#39;manage&#39; and click connect. Now we see the people who&#39;ve registered for the nameday. You see the id of the record on the top right of the row, George&#39;s name and his age. If we click on the row, we can edit this record, for example, we can change his age if we know he lied. Click save and the data is updated. We can pull to refresh if anyone has registered in the meantime and the new records will be displayed. You can swipe left or right to delete a record by pressing the Remove button.

**Hope this helped you and have a nice day!**  :smiley:
