# Passman (easy)

### Challenge Description
Pandora discovered the presence of a mole within the ministry. To proceed with caution, she must obtain the master control password for the ministry, which is stored in a password manager. Can you hack into the password manager?

<br>

### Resources
You are given the application code (javascript application). 

<br>

### Solution

The solution is basically exploiting the fact that the password of a user can be changed without actually being logged in as that user. So you can make a new user and use the change password functionality to change the admin password and then log in to the admin profile to get the flag. 

When you visit the provided IP address you are met with a login form. You can then make a new account.

![alt text](./Screenshot%201.png)

<br>

In the provided code there is a GraphQL query for a password update. That's the functionality you'll use.

![alt text](./Screenshot%2013.png)

<br>

I used a software called Burp Suite (it can be downloaded for free) to intercept the communication between the website and the server and send the query you see in the screenshot below. 

![alt text](./Screenshot%2010.png)

You change the admin password to be anything and then you can login in to the admin account. There you can find the flag as an existing passphrase for the account.

![alt text](./Screenshot%2012.png)

<br>

NB: Burb Suite can seem a bit intimidating to use but there are a lot of guides online on how to work with it.
