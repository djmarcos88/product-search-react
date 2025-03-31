# Product List in React

Objective: Create a list of products on a React app, it has to include pagination and basic token handling.

API Reference: https://dummyjson.com/docs

## Requirements:

This is a standard React app project, check the package.json to find out the script to start the app.

Design the UI with simple CSS, styling is not the main goal of this exercise but it would be nice if you take the time to make things look a bit presentable.

The app already includes a ProductList component. The main goal is to leverage Dummy Json API to create a list of products that is rendered by this component.

The list should contain the following:

-   Lists all the products.
-   Each product card should contain the product title, description, price and thumbnail.
-   The list should handle pagination, only display 10 products per page and include a button to load more upon being pressed.

We also want to see you write functions to handle authentication tokens. The Dummy Json API supports a set of mock endpoints for this.

Thus, the second goal of the exercise is to create a Proxy that runs over your GET products function. It must validate the existing token expiration, and if expired use the refresh token to get a new one.

Your GET products request should utilize the access token as well, to simulate requests that need authorization.

Bonus:

-   Add a dropdown at the top of the page to change the product list sorting order, it should allow to toggle between title and price (only supporting ASC order for the purpose of the exercise is fine).
-   Include a hidden section on each product card that shows the product's reviews, with a button to show or hide it, hidden by default.
