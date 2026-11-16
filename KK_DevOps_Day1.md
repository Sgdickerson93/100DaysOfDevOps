# Linux User Setup with Non-Interactive Shell

Let's get this DevOps party started!

I completed this exercise before, but I quit before I could get deep into the challenge. I'm here to start it over and stick with it.

## What is a Non-interactive Shell?

A non-interactive shell is a shell session that executes a predetermined list of commands or a script automatically without waiting for human input.

### Logging to the server via SSH

https://www.digitalocean.com/community/tutorials/how-to-use-ssh-to-connect-to-a-remote-server

```
ssh username@server_ip
```

### Adding a user using sudo

https://medium.com/@ikunalsingh/create-linux-user-with-non-interactive-shell-332c91cad6ff

```
sudo useradd -s /sbin/nologin <username>
```

### Verify User Addition

```
id mariyam
```
Response:

```
uid=1001(mariyam) gid=1001(mariyam) groups=1001(mariyam)
```

### My Thoughts

EASY. I did ponder the difference between a non-interactive and an interactive shell, as well as their use cases. KodeKloud did provide a good article explaining the difference and the use cases. Advanced Bash Scripting is on my list to learn.

https://notes.kodekloud.com/docs/Advanced-Bash-Scripting/Introduction/Interactive-vs-non-interactive-shell/page

Interactive Mode:
You type commands at a prompt and see immediate feedback.

Non-Interactive Mode:
You place commands in a file (a script) and run them all at once.
