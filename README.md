# Java-II-assingment-3
Assignment 3 – The Facebook Class
Now we’ll continue our project by writing a Facebook class that contains an ArrayList of Facebook user objects. The Facebook class should have methods to list all of the users (i.e. print out their usernames), add a user, delete a user, and get the password hint for a user. You will also need to create a driver program. The driver should create an instance of the Facebook class and display a menu containing five options: list users, add a user, delete a user, get password hint and quit. Then it should read in the user’s choice and call the appropriate method on the Facebook object. This should continue until the user chooses to quit. You don’t need to worry about adding and removing “friends” for this assignment – we’ll do that later in the project.
Here’s the catch: we want the contents of our Facebook object to persist between program executions. To do this, serialize your Facebook object before the program terminates. When the program starts up again, de-serialize the Facebook object rather than creating a new one.
Some details:
When adding a new FacebookUser, prompt the user for the username and check to see that if the users ArrayList already contains a FacebookUser object with that username. If it does, display an error message. If the username is unique, prompt for a password and password hint and create a new FacebookUser object with those values. Add this new user to the users ArrayList.
When deleting a FacebookUser, prompt for the username and check to see that the users ArrayList contains a FacebookUser object with that username. If it doesn’t display an error message. If it does, prompt for the password and check that the FacebookUser object with this username has the same password as the one that was entered. If it doesn’t, display an error message. If the passwords match, delete this FacebookUser object from the users ArrayList.
When retrieving the password hint for a FacebookUser, ask for the username and display an error message if there is no user with that username. Obviously, if the user does exist you should display the password hint without requiring the user’s password.
You will be graded according to the following rubric (each item is worth one point):
• The Facebook class has the appropriate fields and methods
• The Facebook class can list the FacebookUser objects (i.e. their usernames) • It is possible to add a user at runtime
• It is possible to delete a user at runtime
• It is possible to get the password hint for a user at runtime
• The driver program creates a Facebook object that is serialized before the program ends
• The driver program de-serializes the Facebook object when it starts executing, if a serialized version exists. If a serialized version of the Facebook object does not exist, the driver program creates a new Facebook object.
• The program compiles
• The program runs
• The program is clearly written and follows standard coding conventions
