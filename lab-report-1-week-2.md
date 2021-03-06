# Week 1 Lab Report
# 1. Download VS Studio Code
* Visit [VS Studio Code](https://code.visualstudio.com/) and download the version specific to your operating system
* Allow the program to make changes to your device
![Screenshot (212)](https://user-images.githubusercontent.com/97714738/149594512-b2872969-2512-4394-93c4-935c77cf27d7.png)


# 2. Remotely Connect
* First I installed OpenSSH onto my device using Powershell
![Screenshot (214)](https://user-images.githubusercontent.com/97714738/149594721-b847e8d6-c182-4abb-9cb1-eb031589cfe0.png)
* Then I opened VSCode (as an administrator) and entered the command ssh cs15lwi22zz@ieng6.ucsd.edu replacing zz with the numbers in my cse15l account
![Screenshot (215)](https://user-images.githubusercontent.com/97714738/149594908-ce42b428-dd59-4a24-9ca8-878cb7f38590.png)
* When logging in VS Code will prompt you to enter your password
* Enter the password and respond "yes" to the prompt that is output


# 3. Trying some commands
* Enter some commands into the terminal and take note of the output
* Try `ls`, `ls -lat`, `cp /home/linux/ieng6/cs15lwi22/public/hello.txt ~/`, etc.
![Screenshot (217)](https://user-images.githubusercontent.com/97714738/149595641-02271338-7868-4ea8-9b06-3e565f4b7ff8.png)


# 4. Moving files with `scp`
* Create a file WhereAmI.java and save it to the correct directory
* Enter `scp WhereAmI.java cs15lwi22zz@ieng6.ucsd.edu:~/` and then your password
* If no errors, login to your account using ssh and enter `ls`
* The file should be saved in the home directory
![Screenshot (224)](https://user-images.githubusercontent.com/97714738/149597220-5640f9d6-dd2c-47b1-837b-409c60ec57ec.png)


# 5. Setting an ssh key
* Enter the command `ssh-keygen`
* When asked to enter file copy and paste the path in the parentheses
![Screenshot (219)](https://user-images.githubusercontent.com/97714738/149596505-37b3b2a5-9a5b-4a05-bbd7-d9dcd2eaac5f.png)
* Enter the command `ssh cs15lwi22zz@ieng6.ucsd.edu` with your course specific numbers and enter your password
* Enter `mkdir .ssh` then logout
* Finally enter scp with the same path as earlier
![Screenshot (222)](https://user-images.githubusercontent.com/97714738/149596667-b3356a2b-9feb-4d44-8a4e-ac1455aa541f.png)


# 6. Optimizing Remote Running
* Using shortcuts you can optimize running time
* Adding commands in quotes in the terminal after your ssh login will run them automatically after sign in
* Using semicolons in between commands allows you to run multiple commands in the same line
![Screenshot (225)](https://user-images.githubusercontent.com/97714738/149597655-58f07aee-6155-436d-81a1-15494427a621.png)

# 7. Making Remote Running Even More Pleasant
* Including entering my password and using the up arrow to use a previous command, it took me 31 keystrokes to copy the file to the server, login, and then compile and run WhereAmI.java
![Screenshot (262)](https://user-images.githubusercontent.com/97714738/152665330-843bd471-c28b-4d9c-83e6-1ba03b4bf5c3.png)
![Screenshot (263)](https://user-images.githubusercontent.com/97714738/152665336-4fda5898-ab34-4049-b603-89577260c323.png)







Lab 1
ssh login
![Screenshot (209)](https://user-images.githubusercontent.com/97714738/149445964-59cf427a-3df6-425d-a32e-65c736db4c6a.png)



Lab 2 Error Cloning
![Screenshot (203)](https://user-images.githubusercontent.com/97714738/149445550-a8c4b077-5432-458b-9959-6350be97af88.png)
