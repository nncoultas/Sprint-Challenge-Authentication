<!-- Answers to the Short Answer Essay Questions go here -->

1.  Describe Middleware, Sessions (as we know them in express), bcrypt and JWT.

    Middleware: These are functions that can execute code, Make changes to the Request and response objects, end a cycle, and call the next middleware if there is more.

    Sessions: These are from when the user logs in to when the user logs out and the session is terminated.

    Bcrypt: This is a framework that allows us to hash passwords and easily compare passwords

    JWT: JWT stands for JSON Web Token and is a secure way to transmit information. It is also used for Authentication like in this case with allowing a user to access a specific route when having a valid token that the user gets after logging in.

2.  What does bcrypt do in order to prevent attacks?
    Bcrypt let's a password be hashed by multiple rounds and adds more rounds on top of the specified number. This makes it harder for a hacker to gain the password because they have to know the specific number of rounds the password was hashed.

3.  What are the three parts of the JSON Web Token?

    Data - this is the main object you define, in this case it would be the User \_id and username. This is a check to make sure these things are included/verified
    Secret - This is a String unique to the application and something only the server knows. This helps with encryption and decrption.
    Options - This is the length until the Token expires.
