# login-and-password-manager
Simple shell script to help manage your login and passwords


# password_generator

chmod +x password_generator

run it as 

password_generator

It would output two strings, choose either. 
Maybe substitute more special characters with underslashes, if the website places constraints.

# database_creator

Run it as 

database_creator database_file

where database_file is the name of the file you want to store your login credentials in. 

This creates a file/database for storing your site url, login id and password in a proper format.

The last field is populated by tags, tags can be any words or phrases you associate with the website, just put these keywords with a single space between them. If there is error, you can always edit the file manually. Each record is on a seperate line and readable.

After the file is created, store this file carefull, either encrypt it or put it in a safe place.
Always keep a encrypted backup copy somewhere, that is in another computer maybe.

# read_database

Run it as 

read_database database_file

where database_file is the file that you created earlier and in which you stored your credentials.

it would prompy you for a keyword, put in something like facebook or linkedin or reddit or twitter or the special tags that you p ut in earlier. It would grep though the lines and bring up a menu of the relevant login credentials. Choose the one you want.

This action would open the website in firefox and copy your login id into the clipboard via xclip. In the login page, you click the middle mouse button to paste you login id. Go back to the terminal and press enter, this would copy the password to the clipboard or xclip. In the webpage go to the password field and middle click your mouse, thus pasting your password.


# Keep an encrypted copy of the login database file as backup in another physical computer or on a CD.

