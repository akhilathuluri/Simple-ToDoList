# Simple-ToDoList

This documentation provides an overview of the code for a To-Do List application. It explains the structure of the code files, their functionalities, and how they are interconnected. The application allows users to create and manage their to-do lists.

#Code Files

1. **index.html**: This file represents the homepage of the application. It contains the HTML structure for displaying a heading and a paragraph.
2. **list.ejs**: This file is an EJS (Embedded JavaScript) template that is used to render the to-do list view. It includes the "header.ejs" and "footer.ejs" files. It displays the title of the list and the list items dynamically using EJS tags.
3. **about.ejs**: This file is another EJS template used to render the about page view. It includes the "header.ejs" and "footer.ejs" files. It displays information about hummus using HTML markup.
4. **footer.ejs**: This file contains the HTML markup for the footer section of the application.
5. **header.ejs**: This file contains the HTML markup for the header section of the application. It includes the CSS file "styles.css".
6. **styles.css**: This file contains the CSS styles used for styling the application. It defines styles for the HTML elements, such as background colors, fonts, box dimensions, and alignment.
7. **app.js**: This file is the main server-side JavaScript file for the application. It includes the necessary modules, sets up the Express server, defines the routes, and handles the request and response logic.
8. **date.js**: This file is a custom module used to get the current date and format it. It is imported into the "app.js" file to provide the date functionality.
9. **package.json**: This file is a standard Node.js package configuration file. It contains information about the project, its dependencies, and scripts.

## Functionality

1. Rendering the Home Page: The root route ("/") renders the "list.ejs" template with the current date as the list title and the pre-defined items array as the list items. It uses the "date.js" module to get the current date.
2. Adding List Items: Users can add new items to the to-do list by submitting the form in the "list.ejs" template. The form sends a POST request to the root route ("/") with the new item data. The server-side logic in the "app.js" file adds the new item to the items array and redirects the user back to the home page.
3. Rendering the Work List: The "/work" route renders the "list.ejs" template with "Work list" as the list title and the workItems array as the list items. It allows users to manage a separate to-do list for work-related tasks.
4. Adding Work List Items: Users can add new items to the work list by submitting the form in the "list.ejs" template when viewing the work list. The form sends a POST request to the "/work" route with the new item data. The server-side logic in the "app.js" file adds the new item to the workItems array and redirects the user back to the work list page.
5. Rendering the About Page: The "/about" route renders the "about.ejs" template, which displays information about hummus.

## Installation and Usage

To run the To-Do List application locally, follow these steps:

1. Clone the GitHub repository to your local machine.
2. Install Node.js if you haven't already.
3. Open a terminal or command prompt and navigate to the project directory.
4. Run the following command to install the project dependencies:

```
npm install
```
5. Start the application by running the following command:
```
node app.js
```
6. Open a web browser and go to http://localhost:3000 to access the To-Do List application.
7. Use the application to create, manage, and view your to-do lists.

## Conclusion

This documentation provides an overview of the code for a To-Do List application. It explains the structure of the code files, their functionalities, and how they are interconnected. By following the installation and usage instructions, you can run the application locally and use it to manage your to-do lists.
