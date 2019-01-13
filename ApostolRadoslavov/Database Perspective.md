# Database Perspective

The Database perspective contains tools for inspection and manipulation of the artifacts within the underlying relational database. 
It is comprised of the following views:
 - Database View
 - SQL View
 - Result View
 - Console View

The Database perspective features a database explorer, a console to execute SQL statements and to preview results in table format.

![database perspective](http://www.dirigible.io/help/images/ide_perspective_database.png)

# 1. Database View
The Database view gives you direct access to the default target schema assigned to your account in the Web IDE. It enables you to expand the schema item and see the list of all tables and views created either via the data structures models or directly via SQL script. You can further expand each table to view it's columns names and their data types.

![database view](http://www.dirigible.io/help/images/ide_view_database.png)

# 2. SQL View

The SQL view is one of the most powerful and dangerous tool for database management. In the SQL console you can enter the SQL script compliant to the underlying database system. You have the ability to write any type of SQL script. That means you can create tables, views, insert and rows, the lot. You get the result of the execution in the Results view below. 

![SQL View](http://www.dirigible.io/help/images/ide_view_sql.png)

# 3. Result View

The Result view lets you see the result you've got after executing an SQL script. If the script is a query, you will see all the rows which satisfy your query. The Result view will also inform you if there is an error

# 4. Console View
The Console view is a major debugging tool. It displays the output of the code that you are executing. You can see step by step how the script was executed. 

![console view](http://www.dirigible.io/help/images/ide_view_console.png)

If the result from the execution was not what you had expected, you can follow the output code and see what went wrong, making it easier to fix mistakes.
