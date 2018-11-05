**Create and name a new Project**

 1. Start your dirigible.
 
 2. In the window “Workspace Explorer” -> right button on the mouse -> create your new project.
 
 3. Name your project in the gap -> Next -> select the blank application
    template -> Finish.

**Create new Data Structure**

1. Right button on the mouse over the name of the project -> create a new Data Structure

2. Select a Database Table

3. To add all attributes you need choose Add.

**Add attributes in the Data Structure**

1. To define an “ID” attribute as a primary key mark the two boxes – “Not Null?” and “Primary Key?”

2. To choose the type of ID, select INTEGER.

3. To make a database for students:

  - Add FIRST_NAME – type is VARCHAR, length is 30, NOT NULL

- Add LAST_NAME – type is VARCHAR, length is 30, NOT NULL

- Add AVERAGE_GRADE – type is DOUBLE, NOT NULL

- Add BIRTH_DATE - type is DATE, NOT NULL

4. To name your table select Next.

5. The table definitions will be shown in JSON format.

**Publish a Project**

1. To publish your project right button over the name and select Publish.

2. At the top of the screen select “other…” and choose Database in the new opened window.

3. At the SQL Console (at the bottom of the screen) type “SELECT * FROM (name of the table)"

4. Select Query.

5. To see something on the screen add your table in the project.

**Add a table in a Project**

1. Right button over the name of the project and create new Data Structure.

2. Choose “Delimited Separated Values Sample Data” and find the name of your table.

3. To add the table to your project, select Next -> Finish.

4. To publish your project go back on **Publish a Project**.
