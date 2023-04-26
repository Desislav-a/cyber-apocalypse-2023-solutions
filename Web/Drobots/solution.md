# Drobots (very easy)

### Challenge Description
Pandora's latest mission as part of her reconnaissance training is to infiltrate the Drobots firm that was suspected of engaging in illegal activities. Can you help pandora with this task?

<br>

### Resources
You are given the application code (Python application). 

<br>

### Solution

When you visit the provided IP address you are met with a login form. 

![alt text](./Screenshot%201.png)

<br>

From the provided code it can be seen that the form is vulnerable to an injection.

![alt text](./Screenshot%202.png)

<br>

In the form you can then use any SQL injection. For example, **admin** as the username value and **" or ""="** as the password value. That logs you in and you get the flag.

![alt text](./Screenshot%203.png)
