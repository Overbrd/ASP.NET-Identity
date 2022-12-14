# ASP.NET Identity/OWIN Cookie Authentication Log In/Log Out User Authentication Web Forms Project

ASP.NET Web Application built in Visual Studio 2022.

Uses a MS SQL Local DB as the database.

Runs on SQL Server on https://localhost:44349/

Original project instructions are here:

https://github.com/dotnet/AspNetDocs/blob/main/aspnet/identity/overview/getting-started/adding-aspnet-identity-to-an-empty-or-existing-web-forms-project.md

The above project walk-through was based upon using Visual Studio 2017. This source code has been updated to Visual Studio 2022.

Code repo created 09/27/2022 by Matthew C. Lind.

This code was created from a blank project and can be used as a starting point for user authentication projects, and ultimately an .aspx web site.

## Built using .NET 4.7.2.

In order to build this app. with Visual Studio 2022 (using the steps from the link above and this source code) you must follow the directions on the web page below which describes how to install now missing ASP.NET templates for .NET Framework in Visual Studio 2022:

https://www.howtosolutions.net/2021/11/visual-studio-missing-asp-net-web-application-template-dotnet-framework/

### Details

1. Utilizes Identity and Owin packages:

Packages are as follows:

- Microsoft.AspNet.Identity.EntityFramework package

- EntityFramework package

- Microsoft ASP.NET Identity Core package

- Microsoft.AspNet.Identity.Owin package

- Microsoft.Owin.Host.SystemWeb package

2. Includes a web form to register users [Register.aspx]

Basic form for user to input their new chosen user name and password.

If the user name is already taken a warning is given "Name * is already taken."

Password must be at least 6 characters.

If the user name is available the user name and password combination are accepted and a notice is given "Hello *!!" along with a "Logout" button.

If user clicks the "Log out" button they are logged out and referred back to the Login Page.

3. Includes a web form to log in/log out users [Login.aspx]

Basic form for user to input their user name and password.

If the user name/password is correct the user is logged in and receives a "Hello *!!" message and a "Log out" button appears.

If the user name/password is incorrect the user receives a "Invalid username or password" message.

4. LocalDb Identity database and tables are generated by Entity Framework.

5. To view the users table (once one or more users are created successfully) go to 

View->Server Explorer->SQL Server->(localdb)->Databases->WebFormsIdentity->Tables->dbo.AspNetUsers 

then right click on dbo.AspNetUsers->View Data

6. ASP.NET Identity uses the Microsoft OWIN Authentication middleware to conduct forms authentication.

7. The OWIN Cookie Authentication is a cookie and claims-based authentication mechanism and can be used by any framework that is hosted on OWIN or IIS.

8. This same authentication package can be used across many frameworks, including ASP.NET MVC and Web Forms.

9. Cross browser compatible.








