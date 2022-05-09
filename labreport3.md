## Streamlining ssh Configuration
![sshconfig](sshConfig.png)
- I located the .ssh directory and created the config file via VS code with the following:
`Host ieng6
    HostName ieng6.ucsd.edu
    User cs15lsp22akz`
- I decided to not change my alias and leave it as is.

![sshlogin](sshLogin.png)
- Logged in via `ssh ieng6`, a much simpler and quicker command in comparison to `ssh cs15lsp22akz@ieng6.ucsd.edu`

![scpTest](scpTest.png)
- I created a simple scpTest.java file on my desktop via VSCode to test the `scp` command.
- Used the command `scp scpTest.java ieng6`, which copied the source file to the destination.


## Setup Github Access from ieng6
![publicKey](public.png)
- Here I stored the key that I made in lab 1 with the command `ssh-keygen` on my computer.
- I then added it to github by copying the compnents into my github account with the NEW SSH KEY option.

![privateKey](private.png)
![Desktop](1234.png)
- I generated a new private key with `ssh-keygen -t ed25519 -C "kentnguyenn@gmail.com"`.
- It was then stored into my .ssh directory and I was not sure whether to post a picture of it stored on my computer or my github account.

![gitCommands](gitCommand.png)
- I used `git add WhereAmI.java` to add the file WhereAmI.
- I then used `git commit -m "adding a line` to commit a simple line change.

## Copy whole directories with `scp -r`
![markdownCopy](markdownCopy.png)
- I first moved to the markdown-parse directory by opening it on VSCode with github Desktop.
- I then used the command `scp -r . cs15lsp22akz@ieng6.ucsd.edu:~\markdown-parse` to copy the directory onto the remote server.

![markdownServer](markdownServer.png)
- I logged into the server with `ssh ieng6` and then compiled both MarkdownParse.java and MarkdownParseTest.java. with a simple `javac`.
- I then realized I have to compile the tester with the specific Junit command `javac -cp ".;lib\junit-4.13.2.jar;lib\hamcrest-core-1.3.jar" MarkdownParseTest.java`
- After everything worked and tests ran as normal.

![markdownLine](markdownLine.png)
- Combining everything toegether from the first two steps of this section, I added `;` (semicolons) in between each command to run everything in one line.
- `scp -r . cs15lsp22akz@ieng6.ucsd.edu:~\markdown-parse; ssh ieng6 "cd markdown-parse"; cp MarkdownParse.java MarkdownParseTest.java; java -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar org.junit.runner.JUnitCore MarkdownParseTest`
- I am not the biggest fan of doing everything in one line because of the ability to mess up. Still, I would utilize the semi colon to do multiple commands at once.
