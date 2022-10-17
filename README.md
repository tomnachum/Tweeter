# Tweeter Project

## Introduction

In this project, we built the front-end of a tweeter app, using vanillaJS and Jquery.

![Alt text](/images/tweeter.png?raw=true "Optional Title")

## Design

We used MVC architecture pattern as follows:

1. Model.js:
   We implemented basic CRUD operations: read, add and delete a post, and add comments to it.

2. renderer.js:
   We used Jquery to render the posts data, and according to the MVC convention, on each change we render everything from scratch.

3. controller.js
   In the controller we added the event listeners for the add/delete buttons. Important note: at the beginning the posts are not exists in the DOM so we need to add the event listeners dynamically, meaning that the listener will be added to the element in running time after it's creation.

## General notes

- The data is not being saved in local storage or in some DB, this was not the purpse of this exercise. Meaning when refreshing the page or exiting the browser the data will be deleted.
- As desgin requirement empty posts are not allowed.
