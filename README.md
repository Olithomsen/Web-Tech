# My web solution: Front-End

## Introduction

In this assignment, you are tasked with *searching* for a problem, and then designing and creating a web solution for that problem.
The purpose of this assignment is to get you more acquainted with the basics of web development and front-end development: HTML, CSS, and JavaScript.

You must submit your answer to itslearning and ScalableTeaching. We will provide you with dedicated feedback on each submission.
You are allowed to work in pairs, but no more than two!

<span style="color:red">**Disclaimer 1: use of AI** We discourage the use of generative AI to develop this application. The goal of this assignment is to prepare you for the exam, and we will provide feedback on something that **you** make.</span>

<span style="color:red">**Disclaimer 2: exam** We use this and the following assignments as preparation for the exam. We try to be as close as possible to the exam. However, be aware that not every question from the assignments will be present, and we may ask questions that are not included in the assignments.</span>


## Setup

### Questions Submission

In this assignment, you must answer three questions. These questions are provided via assignments using itslearning. The questions are:
* Question 1: Choose the topic
* Question 2: Topic motivation
* Question 3: Why develop a web solution


### Code Submission

We have provided you with a repository (the same one this file is in) through Scalable Teaching, where you will submit any code you create.
Alongside this file, you will find a directory `/solution/` which in turn has three sub-directories:
* `/html/`: In this folder, you should put any `.html` files you create
* `/css/`: In this folder, you should put any `.css` files you create
* `/js/`: In this folder, you should put any `.js` files you create

To submit your assignment, simply push it to the repository. Only the latest push before the deadline will be looked at, so feel free to save your progress as you go.

**Important!**
Remember to double-check that all of your changes are correctly committed and pushed to the GitLab repository we have provided.

## The problem

Before developing a web application, you should start by defining the problem to be solved using web technologies.
During this semester, you are expected to develop a *CRUD*-type of application.

### Task 1: Choose the topic

For example, Miguel uses a *Music Library* application during the semester.
In this application, users can upload music albums, together with information about the album and artists.
If you are out of ideas, you can use one of the following examples:

* Movie Library
* Videogame Library
* E-commerce
* Pet Shelter

### Task 2: Topic motivation

Explain the context behind the chosen topic from the previous task:

* What is the problem?
* What is/are the resource(s) used for this topic (for example, Music Albums for the Music Library topic)
* Who are the users
* Brief description of what the solution should do (in other words, brief description of use cases, we do not expect more than a few paragraphs)

### Task 3: Why develop a web solution

During our course, we learn how to develop applications using web technologies.
However, before even developing one, we should be clear about why we are using a web solution.
In this part, you must explain why your solution should be developed using web technologies, instead of other alternatives (native, mobile, etc.).
To answer this question, we recommend relating the advantages and disadvantages of web applications to the topic's motivation and requirements.

## The application

Now it is the time to build the web application.
For this assignment, you must develop the front-end of the app using HTML, CSS, and JavaScript.
To simplify our application, we will focus on designing the interfaces for CRUD operations.
To do this, your application should consider:

* An index page that allows users to:
	* know they are in the *first page* (in other words, the home page)
	* link to go to another page to create a resource
	* list of all resources currently in the database
		* The information provided for each element should be a summary of the element itself (for example, the music library lists music albums, showing only the name and the artist name, but not the tracks)
		* The first element should have a link to *see more* (a link to the Read operation)
		* The first element should have a link to *edit* (a link to the Update operation)
		* Every element should have a *button* to remove the element from the list, using JavaScript to develop this functionality (this is the Delete operation)
* Create operation:
	* From the index, users can click an option to *create* a new resource
	* This page should have a form that contains all necessary fields to create the resource
	* Use JavaScript to validate every field: if a field is not valid, the submission of the form should fail, and the wrong field should be marked in the form itself
* Read operation:
	* From the index page, only the first element should have a link to *show more* (this is to simplify your development)
	* This page should list all information from the resource
	* Moreover, it should have a link to edit this information (as described in the next point)
* Update operation:
	* From the index page, only the first element should have a link to be editable (this is to simplify your development)
	* This page should have a similar (if not the same) form as the create operation
	* Every field of the form should already be filled with the information of the resource
* Delete operation:
	* As mentioned in the index section, every resource should have a delete button enabled using JavaScript

### Task 0: Interface design and Mock-ups

Before starting to develop, we recommend that you design mock-ups of each interface.
You can use any external tool for this, including but not limited to: [Figma](www.figma.com), [Drawio](draw.io), or even hand-made sketches.

For the design, consider including a header and footer that will be consistent across every page of your application.
This way, there is always a *home* link to go back to the index page of your application.

### Task 1: HTML5

The first step in building your application is to create its structure using HTML.
To do this, you should:

* Build a header and a footer using the proper HTML5 elements
* Write a page for the index, create, read, and update operations
* Connect these pages with links according to the instructions at the start of this section
* Write a form for the create and update pages

### Task 2: CSS

You may notice that your page, while functional, does not look *usable*.
To improve the appearance, you should use CSS.
While you can create any design, we recommend following a proper layout structure (using Flexbox or Grid) and adhering to good practices, such as using red colors for errors (for example, errors on form fields).


### Task 3: JavaScript

Here, you must make your website seem dynamic by implementing several scripts.
Following the instructions at the beginning of this section, you must implement using JavaScript:

* Form validation: Create and Update pages
	* Create and update operations have a form that must be filled with information
	* These fields must be validated if needed
	* If a field is not validated, you should indicate this in the form itself
		* It is up to you how to show the error to the users
* Delete elements: Index page
	* On the list of elements, each element should have a button to remove that element from the list (and that element only!)
