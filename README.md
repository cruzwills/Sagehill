# Sagehill
Sure, here's a sample README file with instructions on how to install and run the application:

Note Taking Web Application
This is a simple note taking web application built using Node.js, Express, MySQL, and React.

Installation
Clone the repository: git clone https://github.com/your-username/note-taking-app.git
Install server dependencies: cd note-taking-app/server && npm install
Install client dependencies: cd ../client && npm install
Configuration
Create a .env file in the server directory with the following environment variables:
DB_HOST=localhost
DB_USER=your-mysql-user
DB_PASSWORD=your-mysql-password
DB_DATABASE=note_taking_app
JWT_SECRET=your-jwt-secret
Replace your-mysql-user, your-mysql-password, and your-jwt-secret with your own values.

Create a MySQL database with the name note_taking_app.

Run the SQL migration scripts to create the users and notes tables:

cd server/sql
mysql -u your-mysql-user -p note_taking_app < 01_create_users_table.sql
mysql -u your-mysql-user -p note_taking_app < 02_create_notes_table.sql
Replace your-mysql-user with your own value.

Usage
Start the server: cd ../server && npm start
In another terminal window, start the client: cd ../client && npm start
Open your browser and go to http://localhost:3000
You should see the registration form. Fill out the form to register a new user, or click on the "Login" link to log in as an existing user.

Once you're logged in, you'll be taken to the dashboard where you can view, add, edit, and delete notes.
