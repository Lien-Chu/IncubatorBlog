+++
title = "Register and Login"
description = "Create a custom signup form!"
draft = true
tags = [  
    "Register",
    "Login",
    "Asp.Net",
    "Database_First"
]
date = "2023-04-04"
image = "https://images.pexels.com/photos/136348/pexels-photo-136348.jpeg?auto=compress&cs=tinysrgb&w=800"
+++

### Let's Create a database first register form:

- Right-click on "Models" and move the mouse to the "Add" button, then a new window with many options appears, click "class...".
![New Class](/IncubatorBlog.io/images/register/add_new_class.png)

- Enter a name for your new class and click "Add". 
![Add Class](/IncubatorBlog.io/images/register/class_name.png)

- Edit new properties in the class file.
![Add Class](/IncubatorBlog.io/images/register/add_properties1.png)
![Add Class](/IncubatorBlog.io/images/register/add_properties2.png)

- Open the file "ApplicationDbContext.cs" in the "Data" folder and add Dbset the new class will just be created.
![Add Dbset](/IncubatorBlog.io/images/register/add_dbset.png)

- Right-click on any of the folders in "Solution Explorer" and move the mouse to the "Add" button, then a new window with many options appears, click "New Scaffolded Item".
![New Scaffolded](/IncubatorBlog.io/images/register/new_scaffolded.png)

- Choose "Identity" and click "Add".
![Add Identity](/IncubatorBlog.io/images/register/Identity.png)

- Select the file of features that you need or choose "Override all files" to select all, choose "Data context class" to "ApplicationDbContext" (Make sure it matches the one added Dbset earlier) and click "Add". 
![Add Identity](/IncubatorBlog.io/images/register/add_identity.png)

- Open "Package Manager Console" from the "Tools" menu at the top of the screen, and enter the following command to add new migration and name it you like then press "Enter".
![Add New Migration](/IncubatorBlog.io/images/register/add_migration.png)
```
PM> Add-Migration "NewMigration"
```

- Enter the following command to update the database and press "Enter".
![update-database](/IncubatorBlog.io/images/register/update_database.png)
```
PM> Update-Database
```
- Let's run the application and see the result.
![run_application](/IncubatorBlog.io/images/register/run_application-1.png)
![run_application](/IncubatorBlog.io/images/register/run_application-2.png)
![run_application](/IncubatorBlog.io/images/register/run_application-3.png)
![run_application](/IncubatorBlog.io/images/register/rigter_confirmation.png)
![run_application](/IncubatorBlog.io/images/register/confirm_email.png)

- Open "Register.cshtml.cs" file in the "Areas" > "Identity" > "Pages " > " Account" > "Manage" folder.
![Edit Register](/IncubatorBlog.io/images/register/edit_register-1.png)

- Add the properties we add to the class file earlier in the "InputModel".
![Edit Register](/IncubatorBlog.io/images/register/edit_register-2.png)

- Modify the class of "CreateUser" method to the class with add the new properties.
![Edit Register](/IncubatorBlog.io/images/register/edit_register-3.png)
![Edit Register](/IncubatorBlog.io/images/register/edit_register-4.png)

- Set these input values to the new properties we created.
![Edit Register](/IncubatorBlog.io/images/register/edit_register-5.png)

- Open "Register.cshtml" file to add the input model to the Register form.
![Edit Register](/IncubatorBlog.io/images/register/register_form-1.png)
![Edit Register](/IncubatorBlog.io/images/register/register_form-2.png)

- before we run the application and see the result, let' updete database again.
![update-database](/IncubatorBlog.io/images/register/update_database_.png)

- Let's run the application and see the result again.
![run_application](/IncubatorBlog.io/images/register/run_application-4.png)
![run_application](/IncubatorBlog.io/images/register/run_application-5.png)
![run_application](/IncubatorBlog.io/images/register/rigter_confirmation.png)
![run_application](/IncubatorBlog.io/images/register/confirm_email.png)


**Congratulations, you have created a custom signup form &nbsp; &nbsp;  ;)**

---



- Go to "View" menu at the top of the screen, and click "SQL Server Object Explorer" from the dropdown menu to open SQL Server Object Explorer.


- Click on "SQL Server" > "(localdb)\MSSQLLocalDB" > "Databases", right click on "Databases" and click "Add New Datadase" to add a new datadase.
![Add New Datadase](/IncubatorBlog.io/images/register/add_new_database.png)

- Enter a name for your New database and click "OK".
![New Datadase Name](/IncubatorBlog.io/images/register/database_name.png)

- Right click on the "New database" that you just created and click "Properties" and copy the value of "Connection String".
![Connection String](/IncubatorBlog.io/images/register/connection_string1.png)

- Go to "Solution Explorer", open "appsettings.json" file, add the "ConnectionString" create a name for it then paste the value.
![Connection String](/IncubatorBlog.io/images/register/connection_string2.png)
![Connection String](/IncubatorBlog.io/images/register/connection_string3.png)



- Enter a name for your New class and click "Add". 
![Add Class](/IncubatorBlog.io/images/register/rename_class.png)

- Edit new properties in the class file.
![Add Class](/IncubatorBlog.io/images/register/add_properties.png)

- Go back to "Solution Explorer", right click on "Solution'ProjectName'" and click on "Manage NuGet Packages for Solution...".
![Manage NuGet](/IncubatorBlog.io/images/register/manage_nuget.png)

- Search keyword "EntityFrameworkCore.Tools" in "Browes" and click "Install".
![Manage NuGet](/IncubatorBlog.io/images/register/sreach_packges_in_browse.png)

- Click on " I Accept" on new window "License Acceptance" to install package.
![Manage NuGet](/IncubatorBlog.io/images/register/accept_license.png)

- Install more packages, then close the "NuGet Solution" window.
1. EntityFrameworkCore.Tools
2. Microsoft.AspNetCore.Identity.EntityFrameworkCore
3. Microsoft.EntityFrameworkCore.SqlServer
4. Microsoft.EntityFrameworkCore
![Manage NuGet](/IncubatorBlog.io/images/register/install_more_packages.png)

- Go to "Tools" menu at the top of the screen, and move the mouse to the "NuGet Package Manager" button, and click "Package Manager Cansole". 
![NuGet Package Manager](/IncubatorBlog.io/images/register/NuGet_package_manager.png)

- Let's run update-database command again.


**Congratulations, you have created your first application in Asp.Net Core.&nbsp; &nbsp;  ;)**

---
