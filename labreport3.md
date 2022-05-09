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

![privateKey](private.png)

![gitCommands](gitCommand.png)

## Copy whole directories with `scp -r`
![markdownCopy](markdownCopy.png)

![markdownServer](markdownServer.png)

![markdownLine](markdownLine.png)
``
