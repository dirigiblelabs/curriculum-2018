# This is a step by step tutorial on how to manage the UI of your project in Eclipse Dirigible and how to create an index page and to add it to the main menu of your web page
## This tutorial is aimed at beginners, but experienced users might find it useful

### Link to a video tutorial
<a href="http://www.youtube.com/watch?feature=player_embedded&v=D6XEs5Zlav4
" target="_blank"><img src="http://img.youtube.com/vi/D6XEs5Zlav4/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>

### Prequisitories: You have a non-empty project with a sample database developed

In this tutorial we will ude the data structures creted in this [tutorial](http://www.youtube.com/watch?feature=player_embedded&v=GwzxjBAhy_4) about how to use data structures in Eclipse Dirigible


23
00:01:48,740 --> 00:01:51,920
In this video, you saw how to manage the UI of 
your project in Eclipse Dirigible.

24
00:01:51,920 --> 00:01:55,560
You learned how to create an index page and to 
add it to the main menu of your web page.




1. Go to the **Workspace Explorer** menu and choose to expand the **ScriptingServices** folder and your project folder after that.

2. Afterward right select your entity and choose from the menu **Generate** -> **User Interface For Entity Service**.

3. Select **List Entities** from the template menu and select **Next**.

4. Following go and right select the new project and choose **New** from the menu and from the next menu choose **Data Structure**.

5. Choose **Select All** button to include all currently available fields in the UI. Continue by selecting **Next**.

6. Type the name of your file. For example "students.html". Select **Next**.

7. Type your page title and choose **Finish**. For example "Students". You have successfully generated a web page showing a list of entries in the database.

8. Now you will learn how to make an index page. Start by going to the **Workspace Explorer** and expanding the **WebContent** folder. Right choose it and select **New** -> **User Interface**.

9. Select **Index Page with Main Menu, Header and Footer** from the template menu and select **Next**. Afterward choose **Next** again.

10. Type your page title and choose **Finish**. For example "University".

11. Open the **main.menu** file in a new tab. In order to expand or minimize the tab window, double-click the **main.menu** tab. 

12. Add the previously generated Students page in the descriptor of the main menu.

For example from this **main.menu**

```sql
[
    {
        "name": "Welcome",
        "link": "index.html",
        "subMenu": []
    },
    {
        "name": "Dropdown",
        "link": "",
        "subMenu": [
            {
                "name": "Form Sample",
                "link": "sample.html"
            }
       ]
    }
]
```
To this:

```sql
[
    {
        "name": "Welcome",
        "link": "index.html",
        "subMenu": []
    },
    {
        "name": "Students",
        "link": "students.html",
        "subMenu": []
    }
]
```

12. Save the changes you have just made.

13. Select the **index.html** file. Open the link generated in the **Preview** tab in a separate browser tab or double-click the **Preview** tab.

14. See what the Students page looks like.

_Hope this tutorial has helped you in how to manage the UI of your project in Eclipse Dirigible!_

_Have a nice day!_ :sunny:
