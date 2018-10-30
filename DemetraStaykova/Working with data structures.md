# Working with Data structures in Eclipse Dirigible

In this tutorial you will learn how to work with Data Structures.

**Context**

        Creating Database.

        Creating Data structure for queries.

**Procedure for creating Database.**

1. In the workspace explorer, select _New_-\&gt;_Project_. Enter the project name.
2. From the menu with templates choose the blank one and select **Finish**.
3. To create a data structure, select your project,_N__ew_-\&gt;_Data structure_.
4. Choose _Relational database table_. Click **Ad**** d** on the left down side of the window.
5. Add 5 columns:

For the first column fill:name - _ID_, type – _integer_, checkbox _N __ot null__?_ and _P__rimary key_. Then select **OK**.

For the second and third column fill: name -_FIRST\_NAME_ _/ LAST\_NAME_, type -_varchar_, _length_ 30, checkbox _N __ot null__?_, then **OK**.

For the fourth column fill: name – _AVERAGE\_AGE_, type –_double_, checkbox _N __ot null__?_

For the last column fill: name –_BIRTHDATE __,_ type– _date_, checkbox  _No__ t__null_? Then select **Next**.

1. Name your table without changing the extension. Then click **Finish**.

As a result, your database is ready.

**Procedure for creating data structure for queries.**

In order to be your queries successful, you need to add another data structure.

1. Select your project,then _New_-\&gt; _Data__structure_.
2. Select the_Delimiter Separated Values_ _(DSV)_ _Sample Data_ template and select **Next**.
3. Find your table and add it to the project, then select **Next**.On the new window, select **Finish**.
4. To publish your project, select your project name and then **Publish**.
5. To open your database view, from the top menu select&quot;_other_&quot; -\&gt; Database.
6. In the _SQL Console_ window, type the _SELECT \* FROM_ command and add _STUDENTS_.
7. Select **Query**.

As a result, some information will be showed. Therefore, your query is successful.