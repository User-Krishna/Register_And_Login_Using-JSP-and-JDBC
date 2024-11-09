<h1>Registration and Login System 🌐🔐</h1>
This project includes two main features: user registration and user login. It uses JSP (Java Server Pages) and Servlets for backend functionality, connecting to a MySQL database to store and validate user details.

<h1>Registration Page (register.jsp) 📝</h1>
The registration page allows users to enter their personal details to create an account. The form includes:

<h3>Name: </h3>The user's full name.
<h3>Email:</h3> A unique identifier for the user (used for login).
<h3>Password:</h3> A secure password for the user’s account.
<h3>Gender: </h3>A choice between Male or Female using radio buttons.
<h3>City:</h3> A dropdown menu to select the user’s city from a list of options (Kathmandu, Rajbiraj, Dharan, Janakpur, Biratnagar).
Once the user submits the form, the details are sent to the Register Servlet (regForm), which inserts the data into the MySQL database. If the registration is successful, a success message is displayed. Otherwise, an error message appears.

<h1>Login Page (login.jsp) 🔑</h1>
The login page allows registered users to log in by entering their email and password. When the user submits their credentials:

1.The Login Servlet (logForm) checks the database for matching credentials.
2.If the email and password match, the user is redirected to the profile page (profile.jsp), where they can see a welcome message with their name.
3.If the credentials do not match, an error message is displayed, and the user is redirected to the registration page.

<h1>Session Management 🖥️</h1>
A session is created for the user upon successful login, and the user's name is stored in the session.
The session name is then displayed in the profile.jsp page as a welcome message.

<h1>Key Technologies Used ⚙️</h1>
<h3>JSP (Java Server Pages):</h3> For creating dynamic web pages.
<h3>Servlets:</h3> To handle form submissions and communicate with the database.
<h3>MySQL:</h3> For storing user registration details.
<h3>HttpSession:</h3> For managing user sessions.
