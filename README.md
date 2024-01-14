MAiL APPLICATION IN PYTHON:-

In First Frame, we need three labels (“Enter Your Credentials”, “Email”, “Password”), two text input entry fields (“Email Entry”, “Password Entry”), and in the last one button for “log in”.

In the Second and Third Frames (we are going to merge them into one window). In the second frame, we have one label (Logged In!) which shows the “logged in” message, and we have one button (“logout”) to log out the user. In the third frame, we have four labels (“Compose Email”, “To”, “Subject”, “Message”), three input fields (“To Entry”, “Subject Entry”, “Message Entry”), and in last we have one button (“Send Email”).

Login( ) Method
In this function, firstly we valid the email and password fields using the validate_login() method. After that, we read the username and password from the entry fields of our GUI. Now make an object of smtplib, and connect with the SMTP server that is running on our machine with default configuration (host = smtp.gmail.com, port = 587). Now login to the server with our credentials (username, password). In the last (on successful login) send a message to the user of login successfully.

Validate_Message( ) Method:
Before sending the email to the recipient, firstly we need to validate the message. In this function, first of all, we read recipient email, subject, and message body from the entry fields. After that, we check that none of them (email, subject, body) is empty, then we check for the valid email using email regular expression.

Send_Email( ) Method:
In this function, we send the email to our recipient. Firstly we need to validate the email, subject, and body using the validate_message() method. After that read the recipient email, subject, and body from the entry field. Now make a message string by combining the username, receiver, subject, and body. In last send the message using the sendmail() method of smtplib

Logout( ) Method:
In this function, we simply quit the connection with the SMTP server using the quit() method. In the last display message of successful log out and end the program.

Main() Method:
In the main method, we set up GUI, ask for user inputs (email and password) and log in to the user. Display appropriate message for login success or failure. After successfully logging in, display the compose email and logout window to the user. Now Ask for user input in the subject, receiver_email, and message body and send an email to the receiver id. In last enable the user to log out from the program and terminate the window by displaying the appropriate message.

Conclusion:
In this tutorial firstly we have learned; what is SMTP, how SMTP server works what is the role of the server and client in SMTP server. Secondly, we created some form of GUI using the Tkinter library of python. Thirdly we implemented some code that we need in sending an email (Login(), Logout(), Send_Email(), etc). We have also gotten to know about App-password. Finally, we run the program and sent an email to our recipient.
In the last, I would love to thank you for your precious time. If you have any queries regarding the project you can send me notes on this article.
