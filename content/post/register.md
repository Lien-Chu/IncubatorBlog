---
date: 2023-04-04
linktitle: Create a custom signup form
description : Create a custom signup form
next: /post/change_database
prev: /post/Hello_World
tags : [  
    "Register form",
    ".Net",
    "Asp.Net"
]
title: Register form
image: "https://images.pexels.com/photos/136348/pexels-photo-136348.jpeg?auto=compress&cs=tinysrgb&w=800"
---

In this article, we will create a custom registration form and add it to the application.


##### Let's Create a database first register form:

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

- Before we run the application and see the result, let's update the database again.
![update-database](/IncubatorBlog.io/images/register/update_database_.png)

- Let's run the application and see the result again.
![run_application](/IncubatorBlog.io/images/register/run_application-4.png)
![run_application](/IncubatorBlog.io/images/register/run_application-5.png)
![run_application](/IncubatorBlog.io/images/register/rigter_confirmation.png)
![run_application](/IncubatorBlog.io/images/register/confirm_email.png)


##### Congratulations, you have created a custom signup form &nbsp; &nbsp;  ;)

---

