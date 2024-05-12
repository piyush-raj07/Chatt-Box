
# Real Chatt Application

This project is a real-time chat application built using Node.js, Express.js, Socket.IO, and MySQL. It allows users to register, login, and engage in real-time text-based communication with other users. The application features user authentication, session management, and dynamic updating of messages without the need for page reloads. 


## Setup and Run Instructions:

1. Install Node.js if not already installed.

2. Clone or download the project from the repository.

3. Navigate to the project directory in the terminal.

4. Run npm install to install the required dependencies.

5. Start the server by running node app.js

6. Open a web browser and navigate to http://     localhost:3000 to access the application.

## API Route Descriptions:

-> GET /index: Renders the login page.

-> GET /register: Renders the registration page.

-> POST /logindata: Handles user login. Expects email and password in the request body. If the provided credentials match a record in the database, the user is redirected to the search page; otherwise, an error page is rendered.

-> POST /register: Handles user registration. Expects email and password in the request body. Inserts the user data into the database and renders the login page upon successful registration.

## Environment Configurations:

-> Express.js: Used for creating the web server and handling HTTP  requests.  
npm install Express

-> Body-parser: Middleware for parsing request 
                 bodies.   
 
-> Multer: Middleware for handling multipart/form-data, used for file uploads.  
 npm install Multer     

-> MySQL: Database management system used for storing user data.    
npm install MySQL

-> Express-session: Middleware for managing user sessions.    
 npm install express-session

-> Socket.IO: Library for enabling real-time 
      bidirectional  event-based communication.  
       npm install Socket.io


## Additional Notes

->The app.js file contains the server-side logic, including route handling and Socket.IO integration.

->The index.html, register.ejs, and search.ejs files contain the HTML templates for the login, registration, and search pages, respectively.

->CSS styles are embedded within the HTML files for simplicity. However, it's recommended to separate them into external CSS files for better maintainability.

->Ensure that your MySQL database is properly configured with the necessary tables for user authentication and registration.
