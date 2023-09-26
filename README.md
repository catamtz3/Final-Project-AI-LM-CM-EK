# Project Overview
An inventory management web service for a video game store.
The project utilizes a simple back-end API (via REST and GraphQL) that allows the users to interact with the game stores inventory.
The project is based off of a given MySQL Database with the given tables:
Games
Consoles
T-Shirts
Invoice
Fees
Taxes

We deployed on Amazon RDS and used a Circle CI/CD set up for continuous integration and development of the project.

# Project Design: What We Need to Account For
The REST API needs to provide the following features for each of the tables:
Standard CRUD operations
Search operations by specific attributes
Example: Get Consoles by manufacturer, Get T-Shirt by Color, etc.

GraphQL queries need to allow users to retrieve information about games and consoles.

# Project Design: How We Designed the Project to Suit Our Needs
We built a spring boot web project to broadcast our web server and allow us to edit via IntelliJ
Created models to hold the databases tables information in Java
Created repositories to connect the MySQL database to our application
Created controllers to handle user requests/responses
Created a service layer and view model to handle the invoice table
    The invoice table interacts with the fees and taxes table, Service Layer handles these transactions
    View Model handles the information for these transactions


