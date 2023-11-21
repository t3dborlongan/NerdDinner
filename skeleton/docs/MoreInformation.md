The best way to learn a new framework is to build something with it. This tutorial walks through how to build a small, but complete, application using ASP.NET MVC, and introduces some of the core concepts behind it.

The application we are going to build is called "NerdDinner". NerdDinner provides an easy way for people to find and organize dinners online:

Screenshot of the Nerd Dinner application page. The Host a Dinner page is shown.

NerdDinner enables registered users to create, edit and delete dinners. It enforces a consistent set of validation and business rules across the application:

Screenshot of the Nerd Dinner application page. The Edit Dinner page is shown.

Visitors can use an AJAX-based map to search for upcoming dinners being held near them:

Screenshot of the Nerd Dinner A J A X based map page.

Clicking a dinner will take them to a details page where they can learn more about it:

Screenshot of the Nerd Dinner web page with details about the A S P dot NET Study Group dinner.

If they are interested in attending the dinner they can login or register on the site:

Screenshot of the Nerd Dinner Log On page.

They can then click an AJAX-based RSVP link to attend the event:

Screenshot of the Nerd Dinner Study Group page. The R S V P button can be found at the bottom.

Screenshot of the Nerd Dinner details page. A message saying Thanks we'll see you there is shown.

Implementing NerdDinner
We are going to begin our NerdDinner application by using the File->New Project command within Visual Studio to create a brand new ASP.NET MVC project. We will then incrementally add functionality and features. Along the way we'll cover:

How to create a new ASP.NET MVC Project
How to create a database
How to build a model with business rule validations
How to use controllers and views to implement a listing/details UI
How to provide CRUD (create, read, update, delete) data form entry support
How to use ViewData and implement ViewModel classes
How to re-use UI using master pages and partials
How to implement efficient data paging
How to secure applications using authentication and authorization
How to use AJAX to deliver dynamic updates
How to use AJAX to implement mapping scenarios
How to enable automated unit testing
You can build your own copy of NerdDinner from scratch by completing each step we walkthrough in this chapter. Alternatively, you can download a completed version of the source code here: NerdDinner on GitHub. You can also optionally also download a free PDF version of this tutorial if you want to read the tutorial offline.

You can use either Visual Studio 2008 or the free Visual Web Developer 2008 Express to build the application. You can use either SQL Server or the free SQL Server Express for the database.

You can install ASP.NET MVC, Visual Web Developer 2008 Express, and SQL Server Express (all free) using V2 of the Microsoft Web Platform Installer

Now let's get started....
Now that we've covered what NerdDinner is, let's roll up our sleeves and write some code.

We'll begin by using File->New Project within Visual Studio to create the NerdDinner application.


