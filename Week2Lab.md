
# Installing VS Code
![VSCode](vscode.png)
- Installing VS code was easy, simply navigated to the VS code website and then installed the program.
- Attached is my VS code startup window.

# Remotely Connecting
![Remote](RemoteConnect.png)
- I am on MacOS so I did not have to install OpenSSH, but I did have to prepare my course-specific account for CSE 15L by resetting the password.
- I connected to the server through my local device with $ssh cs15lsp22akz@ieng6.ucsd.edu.
- I had to answer some simple questions and ended up getting connected as shown in the screenshot above.

# Trying Some Commands
![Commands]()
- I began with trying out the command 'cd ~', which allows the user to change their working directory.
- I then tried out two commands 'cp /home/linux/ieng6/cs15lsp22/public/hello.txt ~/' and 'cat /home/linux/ieng6/cs15lsp22/public/hello.txt', but my permission was denied.
- The first command allows the user to copy files or directories, while the second command allows the user to concatenate files.
- I also tried ls which is a command that lists files.

# Moving Files with scp
![Moving](Moving.png)
- Created a file called WhereAmI.java
- Moved the file from my local device to the server.

# Setting an SSH Key
![SSH](SSH.png)
- Created an SSH Key for my device.
- Able to login without a password.

# Optimizing Remote Running
![Optimize](Optimize.png)
- Able to edit and run WhereAmI.java quicker without entering in a password each time.
- Saved ~10 seconds.
