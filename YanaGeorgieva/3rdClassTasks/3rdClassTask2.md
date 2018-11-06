# This is a step by step tutorial on how to use the basic data structures in Eclipse Dirigible
## This tutorial is aimed at beginners, but experienced users might find it useful

### Link to a video tutorial
<a href="http://www.youtube.com/watch?feature=player_embedded&v=GwzxjBAhy_4
" target="_blank"><img src="http://img.youtube.com/vi/GwzxjBAhy_4/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>


1. Go to Eclipse Dirigible Web IDE.

2. Afterward go to the **File** menu located in the upper left corner and choose **New** and select **Project** and name it.

3. Choose the blank application template from the menu. Choose **Finish** to end the creation of the project.

4. Right-click the new project and choose **New** from the menu and from the its menu choose **Data Structure**.

5. Time to create the database. Select the **Relative Database Table** template from the menu. Click **Next**. On this step you must add all necessary table properties like naming the table and adding the types of columns. 

6. How to create column? If we assume your table is going to hold the essential data of a university student. It will need to have a column for a faculty number, a name (First and Last), an average grade and a column for the birth date. Add a column for a faculty number (FN for short). Click the **Add** button and start filling off the fields:
+ **Name**: ID
+ **Type**: INTEGER
+ Check boxes **Not Null?** and **Primary key?**

_You see we have let some field intentionally black. That is because we won't be needing the faculty number to have a maximum length allowed (it is for **VARCHAR**) and because it is a primary key it won't be needing a default value._

For the rest of the columns fill in:
+ **Name**: FIRST_NAME
+ **Type**: VARCHAR
+ **Length**: 30
+ Check boxes **Not Null?** and **Primary key?**

------

+ **Name**: LAST_NAME
+ **Type**: VARCHAR
+ **Length**: 30
+ Check boxes **Not Null?** and **Primary key?**

------

+ **Name**: AVERAGE_GRADE
+ **Type**: DOUBLE
+ Check boxes **Not Null?** and **Primary key?**

------

+ **Name**: BIRTH_DATE
+ **Type**: DATE
+ Check boxes **Not Null?** and **Primary key?**

------

7. After filling all the necessary columns for your table, select **Next** and name your table (let the name be STUDENTS for example). Afterward click **Finish**.
_For the curious the table definitions are written in **JSON** format._

8. Go again to the name of the project and right-click it and choose from the menu **Publish**. Select the button **other..** located in the left top part of the screen near the logo. Choose from its menu **Database**. You have successfully published your database and activated the SQL console so you can have a way to view and manipulate our data. But if we try to retrieve any data any query will retrieve nothing. That's because your table is empty and you need sample data.

9. We need sample data. Let's go and create another **Data Structure**. This time from the template menu select **Delimiter Separated Value Sample Data** and choose **Next**. Find a table with the name **STUDENTS** which holds sample data appropriate for our table and select it. To finish choose **Next** and **Finish**.

10. Publish the updated version of the database and activate the SQL console. Let's try to query it with **SELECT * FROM STUDENTS;**. Voilà! This time you succeeded it retrieving data from the table.

_Hope this tutorial has helped you in how to create basic data structures in Eclipse Dirigible!_

_Have a nice day!_ :sunny:
