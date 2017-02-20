# Wardrobe

## Overview

Create a database-first web application for managing the contents of your wardrobe. The app will allow you to add, edit, view, and delete items in your closet.

## Due

This project is due **Monday 2/20/2017, at 12:00 PM**. 

## Tasks

### Required Tasks

- [ ] Project Setup
  - [ ] Create a project/repository called `wardrobe`
  - [ ] Create a README.md file explaining what this project will involve
- [ ] Organization of clothing by type
  - [ ] Tops
  - [ ] Bottoms
  - [ ] Shoes
  - [ ] Accessories
- [ ] Controllers
  - [ ] For each model
- [ ] Views
  - [ ] Tops
  - [ ] Bottoms
  - [ ] Shoes
  - [ ] Accessories
  - [ ] Customize the index/detail views to properly show the properties of each item
  - [ ] Have a photo displayed for each item on the details view (The images do not need to be unique)
  - [ ] /Home/Index.cshtml should be updated for your app
- [ ] Bootstrap/CSS
  - [ ] Updated navbar
  - [ ] Thumbnails
  - [ ] At least 3 other Bootstrap components of your choice
  - [ ] Responsive layout

### Stretch Tasks

- [ ] Have the images for each item display on the index view
- [ ] Outfit Model
- [ ] Integrated views with the Outfits model
  - [ ] Show several pieces of clothing from your model on one view

## Details

Design an app that will let you manage the contents of your closet. It should support several different types of clothing stored in your database:

- Tops
- Bottoms
- Shoes
- Accessories

Whether or not you store these as separate tables or a single table is up to you. You will need to have views that allow the user to focus on clothing by type, so keep that in mind when making your decision.

Each item of clothing will need to have the following properties kept with it:
- ID
- Name
- Photo
- Type
- Color
- Season
- Occasion

For the photo, you should use an `nvarchar` column type, and put all photos in the `Content` folder of your project. Save a relative URL of the form `~/Content/myphoto.jpg`, and use that as the `src` of an `<img>` tag in your view file. Be sure to use the Razor method `@Url.Content()` method when calling the relative paths.

You need to determine the appropriate columns/constraints to use for all the other fields.

You should customize all of your views to develop the best user experience you can manage. Use Bootstrap effectively to make the app responsive for both desktops and mobile devices. Add your own styles to make it a little less "bootstrappy".


### Stretch Tasks

A natural progression of this app is to support the creation of outfits - a collection of coordinating tops/bottoms/shoes/accessories. Build this into your model, and create views for working with outfits.

Ultimately, your views should be integrated, so you can see all the pictures of each item per outfit.


## Hints

As usual, start with the model, and spend some time considering how many tables to create and how they will be related. Remember, "it's cheaper to make mistakes on paper first."

Use the scaffolded controller views to get going and put some data in your app, and then start to work on the index view(s) and making them look nice.

Always target MVP - and once you get there, figure out what the next MVP is!

Use dropdowns when you want to limit a user's possible choices. There's an HTML element that lets you do this!


* [Submission Link](https://docs.google.com/forms/d/e/1FAIpQLSdXw1dK-mhJnMCVWC7VMYqoiiK2IOVn8AXn_8ZQCQqiUxKQJg/viewform)*
