---
date: 2023-04-12
linktitle: Create Admin & User Role 
description : Ensure that users only have access to the parts of the application
tags : [  
    "Admin Role",
    "ASP.NET CORE MVC"
]
title: Create Admin & User Role 
image: "https://images.pexels.com/photos/1033142/pexels-photo-1033142.jpeg?auto=compress&cs=tinysrgb&w=900"
---
##### What are the Admin and User roles in ASP.NET used for? 

The Admin and User roles are used to control access to different areas of a web application based on the user's role.

The Admin role typically has access to all areas of the application, including sensitive administrative functions such as user management, system settings, and other restricted areas.

The User role, on the other hand, typically has limited access to the application and can only perform certain actions or access certain areas of the application. For example, a User may only be able to view or edit their own profile information, view public content, or submit requests through the application.

By setting up these roles can control access to sensitive information and ensure that users only have access to the parts of the application that they are authorized to use. This helps to enhance security and protect against unauthorized access or misuse of the application.

- Add a new folder to the project called "Constans" and add a new class called "Roles.cs"
![Constans Folder](/IncubatorBlog.io/images/admin_&_user/add_constans_folder.png)
![Roles.cs](/IncubatorBlog.io/images/admin_&_user/add_roles_class.png)

- Add the following code to the Roles.cs class:
![Roles.cs](/IncubatorBlog.io/images/admin_&_user/add-new_roles.png)

- Add a new class to the "Data" folder called "Dbseeder.cs"
![Dbseeder Folder](/IncubatorBlog.io/images/admin_&_user/add_dbseeder.png)

- Add the following code to the "Dbseeder.cs" class to create the Admin role set the password for the Admin.
![Dbseeder](/IncubatorBlog.io/images/admin_&_user/dbseeder.png)

- Assing roles to users in "Register.cshtml.cs" class
![Register.cshtml.cs](/IncubatorBlog.io/images/admin_&_user/assing_role_to_user.png)

- Modify Identity configuration in "Program.cs" class
![Program.cs](/IncubatorBlog.io/images/admin_&_user/modify_config-1.png)
![Program.cs](/IncubatorBlog.io/images/admin_&_user/modify_config-2.png)

- Modify user link in "Shared/_LoginPartial.cshtml/" class
![_LoginPartial.cshtml](/IncubatorBlog.io/images/admin_&_user/modify_user_link-1.png)
![_LoginPartial.cshtml](/IncubatorBlog.io/images/admin_&_user/modify_user_link-2.png)

- Let's test the application to see if the admin role is logged in properly.
![Admin Role](/IncubatorBlog.io/images/admin_&_user/admin_login-1.png)
![Admin Role](/IncubatorBlog.io/images/admin_&_user/admin_login-2.png)

- Let's test the application to see if the user role is logged in properly.
![User Role](/IncubatorBlog.io/images/admin_&_user/user_login-1.png)
![User Role](/IncubatorBlog.io/images/admin_&_user/user_login-2.png)

- Great! We have successfully created the Admin and User roles in ASP.NET Core MVC. Now we can comment out the code only use once for creating the Admin role in the "Program.cs" file.
![Program.cs](/IncubatorBlog.io/images/admin_&_user/comment_code.png)


##### Congratulations, you have Changed Admin & User Role &nbsp; &nbsp;  ;)

---

*In this article, we refer to Ravindra Devrani's Youtube channel*

[Shopping Cart project in .net core mvc (with authentication) | part 2](https://youtu.be/Z8Vx3bn8AR8)* 

---
