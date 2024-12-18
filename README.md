# Project introduction

The "FoodBank" platform is a comprehensive web application designed to enhance engagement and management within volunteer organizations.\
This platform will enable users to seamlessly sign up, log in, and interact with their respective volunteer organizations through a variety of intuitive features.\
Leveraging technologies such as NodeJS, Express, Vue.JS, and AJAX, alongside a MySQL database, our application aims to provide a robust and accessible environment for both volunteers and organization managers.

## Home Page
![image](https://github.com/user-attachments/assets/d6ca591d-8616-480f-8222-625f5553b860)

## Branch Location
![image](https://github.com/user-attachments/assets/b793ed26-9aca-4bf3-9cb5-b61a75242b49)

## About Page
![image](https://github.com/user-attachments/assets/456f7700-6bb3-4d09-a90c-af9e94b43998)

## Login Page
![image](https://github.com/user-attachments/assets/6868cb4a-9988-4524-82b8-b03521a13c1d)

## User Page
![image](https://github.com/user-attachments/assets/55f29692-004c-419d-8c10-dbbce6e176c5)

## Manager Page
![image](https://github.com/user-attachments/assets/4ebabd3e-66fe-4011-95d1-db10a35f12e4)

## Administrator Page
![image](https://github.com/user-attachments/assets/401232af-e431-4db8-a5fc-14444a5a1aeb)

A demo video is avaliable on YouTube [FoodBank Organization Platform Demo](https://www.youtube.com/watch?v=SKAsz3ZzhVY).

# Environmental dependence
 Windows 10 or later, macOS Catalina or later, or any of the current major Linux distributions are recommended.

# Sample login email and password
Since all passwords in FoodBank.sql are salted, we provide some unsalted password for testing:
### User Table
1. **JohnDoe**: `johndoe@example.com` / `hfeuiah32323`
2. **JaneDoe**: `janedoe@example.com` / `fjoaije2143`
3. **AliceJohnson**: `alicej@example.com` / `dfpkrpokgopr7868`
4. **BobSmith**: `bobsmith@example.com` / `fejoaifjei7658`

### Manager Table
1. **JohnDoe**: `johndoe@example.com` / `fihuewhiu49874`
2. **JaneDoe**: `janedoe@example.com` / `fjdoiajfio3490`
3. **AliceJohnson**: `alicej@example.com` / `froihri4ueh39289`
4. **BobSmith**: `bobsmith@example.com` / `fnirhoiorjeio4839`

### Administrator Table
1. **JohnDoe**: `johndoe@example.com` / `fihuewhiu49874`


# Instructions for use
 1. Start the Docker environment
 2. Starting the mysql Service:`service mysql start`
 3. Migrate the database according to FoodBank.sql
 4. Start the project on port 3018:`node app.js`

# Version updates
##### v0.0.1-k: Static File Implementation: index.html,about.html,location.html,login.html,register.html.
##### v0.0.2-k: Create the Branches table and implement location.html to dynamically update the name and location of the organization's branches by querying the Branches table.
##### v0.0.3-w: Preliminarily created a database relationship diagram, and based on the relationship diagram, initially created user, administrator, activity, and other connection tables.
##### v0.0.3-w: The user profile interface is initially completed; after the initial registration information, the user still needs to add more information to complete the registration interface, and the personal profile interface can only be entered after the registration is completely completed.
##### v0.0.4-k: Separate the database connection file db.js, delete unnecessary files, complete the back-end logon logic, and jump to user.html after success.
##### v0.0.4-k: Create manager registration and login page, implement back-end logon and registration logic; Create an administrator login page to implement the back-end login logic.
##### v0.0.5-j: Implemented the member data management of the branch administrator, allowing administrators to add, edit, and delete member data.
##### v0.0.6-j: The file structure has been modified to ensure consistency with the main branch, using a new database structure.
##### v0.0.7-j: Use cookie and JWT to verify manager's identity. Manager will not be able to login or fetch the member data if not verified.
##### v0.0.8-z: Finish features of administrator, including editing, adding and deleting users.
##### v0.0.9-j: Merged the branch of manager and administrator, applied JWT verification to both manager and administrator login strategy.
##### v0.0.10-w: Improved the personal profile interface, including the ability to change avatars and edit personal profile information. Users can now change their passwords with added requirements for password security levels and restrictions to ensure passwords are not the same as before.
##### v0.0.11-w: Implemented partial refresh and modal box functionality for user interface elements. Enhanced the display of user information on active pages, providing a more dynamic and seamless user experience.
##### v0.0.12-z: Finish features of administrator, including editing, adding and managers and branches.
##### v0.0.13-z: In adding users, organization, branch or administrator: setting to pop up a table to let popole operate.
##### v0.0.14-j: Completed the update post functionality for the branch manager section and improved the corresponding database logic. Now, the manager can choose to publish notifications as public, inside branch, or private categories.
##### v0.0.15-j: Improved and integrated the UI design for the manager section, ensuring consistency between the manager and administrator UI. Updated the CSS for the footer section.
##### v0.0.16-j: The authentication part of the entire management system has been completed using cookie-parser. Upon successful login, the system places the token in a cookie and sends it to the client.
##### v0.0.17-k: Use regular expressions to verify email format and password length when users and managers register, and make correct prompts.
##### v0.0.18-k: Complete third-party login
##### v0.0.19-k: Use twitter-api-v2 to synchronize activity information to Twitter after the administrator adds an activity.
##### v0.0.20-k: Modify the project's registration and login logic, use hashing and salting to save and verify passwords.
##### v0.0.21-k: Add branch_details.html to display branch introductions and announcements
##### v0.0.22-j: Implemented email notifications via Google's OAuth2: an email will be sent to the branch members when a post is updated or an event is held.
##### v0.0.23-j: Integrated with the user management section and refactored the User interface using Vue.js.
##### v0.0.24-z: Completed the RSVP section and made corresponding modifications to the database. Branch managers can now view RSVP information for different events.
##### v0.0.25-z: Finish the connection of administrator to the database, including when editing, adding or deleting users, the database updates too.
##### v0.0.26-z: Finish features of administrator, including sign up other administrators.
##### v0.0.27-z: Finish the connection of administrator to the database, including when editing, adding or deleting managers and branches, the database updates too.
##### v0.0.28-z: Finish the connection of administrator to the database, including when signing up other administrators, the database updates too.
##### v0.0.29-j: Fixed en error of register and third-party login section, now the token would be correctly sent.
##### v0.0.30-k: Update AddDetail.html to dynamically obtain branch information and optimize registration logic.
##### v0.0.31-j: Fixed error in rsvp of manager system and profile.
##### v0.0.32-j: Finished the presentation video.
