---
date: 2023-04-06
linktitle: Change Database
next: 
prev: /post/register_and_login
tags : [   
    "Asp.net core",
    "Database"
]
title: Change Database
image: "https://images.pexels.com/photos/3137068/pexels-photo-3137068.jpeg?auto=compress&cs=tinysrgb&w=800"
---

Now that we have a custom registration form, we need to change the database if we want to save the data in a specific database. In this article, we will change the database created in one article to another database of ours.

##### Let's check the existing database in SQL Server Object Explorer:

- Go to "View" menu at the top of the screen, and click "SQL Server Object Explorer" from the dropdown menu to open SQL Server Object Explorer.
![SQL Server Object Explorer](/IncubatorBlog.io/images/change_database/sql_server_object_explorer.png)

- Click on the "SQL Server" > "(localdb)\MSSQLLocalDB" > "Databases" > "aspnet-yourProjectName" then right-click "Properties" and you can see the value of "Connection String" is match with data in "appsettings.json" file in "Solution Explorer".
![Connection String](/IncubatorBlog.io/images/change_database/connection_string.png)
![Connection String](/IncubatorBlog.io/images/change_database/appsettings_json.png)



##### Let's change database to the one you mant:

- All you need to do is change the value of "Connection String" in "appsettings.json" file to the value of "Connection String" of the database you want to change to.
![Connection String](/IncubatorBlog.io/images/change_database/change_connection_string.png)

- Then update the new database.
![update-database](/IncubatorBlog.io/images/register/update_database_.png)
```
PM> Update-Database
```

*Please be aware that if there is a password included in your connection string, you may need to manually re-enter the password after copying and pasting the string.*


**Congratulations, you have Changed database &nbsp; &nbsp;  ;)**

---

