# Fortune Teller MVC

## Overview

Create a SQL database and table(s) to represent the information a fortune teller would gather, and create the Visual Studio MVC project to allow you to work with/present the information in the database.

## Tasks

### Required Tasks

- [ ] Yak Shaving
  - [ ] Create a Visual Studio project named `fortune-teller-mvc`
  - [ ] Make frequent commits with descriptive messages
- [ ] Database Design
  - [ ] Create a database called `FortuneTellerMVC`
  - [ ] Create the `Customers` table
    - [ ] `FirstName`
    - [ ] `LastName`
    - [ ] `Age`
    - [ ] `BirthMonth`
    - [ ] `FavoriteColor`
    - [ ] `NumberOfSiblings`
  - [ ] Create any other necessary tables and link them
  - [ ] Generate the SQL for the database schema
- [ ] Link Database with Project
  - [ ] Add model linked to database
  - [ ] Add a controller for `Customers`
  - [ ] Add a link to the Home/Index view to access the `Customers` controller
  - [ ] Add the database schema `SQL` file to your project
- [ ] Fortune (`Details`) page
  - [ ] Modify the `Details` action (controller method) and view to display all the fortune information, based on the information in the `Customers` table

### Stretch Tasks

- [ ] Spruce up your view files

## Details

For this assignment, you will go through the process of creating a SQL database, creating an MVC project, and linking them together. This is known as the "database first" method of developing a site. We will focus on a problem that we have already solved using a console application: the Fortune Teller project.

We'll start by storing the data, then look at implementing the logic.

Start by creating a new project in Visual Studio that is an **ASP.NET Web Application** using the **MVC** template.

Then in SQL Server Management Studio, design your database. Make sure to create a new database for this project called `FortuneTellerMVC`, then create a table for `Customers`. Make sure it has appropriate columns with appropriate data types. Create any additional tables necessary to match your database design.

Back in Visual Studio, you need to link the database to your project. Do this by first adding a new **ADO.Net entity data model** using **EF Designer from Database**, selecting your database as the data source.

After confirming that your table is showing up in the Entity Framework designer, create a controller.

Next, open up the `Index.cshtml` file in the `Views/Home` folder. Add a link to your new controller in this file and test out your controller!

Also, you should export your database schema. This can be done from SQL Server Management Studio by right-clicking on the database, choosing `Tasks` > `Generate scripts`.

![Generate SQL scripts](generatesql.gif)

Save the SQL file to your project folder and make sure it is committed to your repository using `git add` and `git commit`.

### Fortune (Details) page

To actually show customers their fortunes, we're going to modify the `Details` page for a Customer object. That's going to involve changing things in two files: the Controller file and the View file.

Your "business logic" goes in the controller. Find the `Details` method of the `Customers` controller. It already has been scaffolded to look up some information about a `Customer`. To pass extra information, you can use the `ViewBag`, a _dynamic_ object.

Before you `return View`, you can put information in the `ViewBag`. For example, to add a property called `RetirementAge`, put the following in the `Details` action method:

```cs
ViewBag.RetirementAge = 75;
```

Don't sweat the details about dynamics just yet - we'll discuss them more. Basically, think of them like objects that can have any properties you want them to have. To access the property in the `cshtml` file, you can do something like this:

```html
<p>You will retire in <span>@ViewBag.RetirementAge</span> years</p>
```

The `@` character puts your `cshtml` file into "Razor mode", where it evaluates C# as it loads the view. The code above just pulls the property out of the `ViewBag` called `RetirementAge` and sticks it in the HTML. Having it in the `<span>` is semi-optional, but makes it clearer to Razor where the C# portion ends.


### Stretch Tasks

Explore the `cshtml` files that make up your application and make them look a little bit better. The `Shared/_Layout.cshtml` is included on every page of your site, and the `Content/Site.css` file lets you easily include CSS customizations beyond Bootstrap.


## Hints

This assignment is _very similar_ to the task you did when learning database first MVC, with a simpler database schema. To start with, just worry about getting the database and basic controller actions set up! Everything else will follow from that.

* [Submission Link](https://goo.gl/forms/klAY4tUOb1Kw9xdq1)*
