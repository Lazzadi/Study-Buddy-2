# Study-Buddy-2
Deployed to Heroku : https://nameless-inlet-58985.herokuapp.com/


I. Description

This project is a Django application that allows users to create rooms based on various topics and start conversations in those respective rooms. The back-end component is done in Python while front-end is a combination of HTML, CSS and JavaScript.

II. Ways of working

First, I built the basic templates in HTML for the home page, room display page, the feed component and the room component that are displayed along the main content, along with the URLs and views. After that I created the database for users, rooms and messages.

After that I created a search functionality that looks after room names and can accept partial inputs and display results (e.g. for "jav" it will display the rooms Java and JavaScript).

The most challanging part was the registration, login, logout functionalities and restricting content based on user login status.

As my focus was mainly on the backend, the CSS was taken from another project and will be addapted in a future version.


III. Navigting the project

There is no need to login to view rooms and conversations, however the "create a room" button will redirect an unlogged in user to the login page. User can create an account at the registration page and then create rooms and add comments to other rooms. Only a user can delete their own room/comment from the website.

The website is also mobile responsive, collapsing the 2 feeds on either side into 2 buttons that access pages which reveal the activity feed and the topic list.

IV. The code

The folder structure is set up by the Django framework and follows a views, templates and models architecture:
	views - contains the backend functionality of a page and gives the context and elements that will be rendered by the HTML

	templates - contains the HTML pages that receive information from the views file

	models - contains the Topic, Room and Messages database models. The User model is imported from the Django database having just username and password elements

	urls - creates the path to access the template and connects the template with the view


V. Issues and problems encountered

The biggest issue is not necesarily the logic of the program, as the backend uses simple if/else and for statements. The main challange was understanding the Django framework and functionalities as well as learning about the built in models and functions. 

However, after building the first model-template-view relation and connecting them through URLs, repeating the process proved easier.

VI. Future features/fixes I would like to implement:

	Create a user_profile model separate from the user model provided by django that would include more user information such as full name, description, favourite programming languages and profile picture

	Fix the overlap on the activity feed on the mobile view

	Populate the models with dummy data in order to have a better idea of how the site responds when there is a lot of data to show.
