*The password for the next level is stored in a file called **readme** located in the home directory. Use this password to log into bandit1 using SSH. Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.*

Use ssh command to connect to a remote host.

```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
```

Password: bandit0
If you use windows you can connect through Putty(free SSH and Telnet client, https://www.putty.org/)

### Solution 1
```bash
cat readme
```

### Solution 2
```bash
more readme
```

Password for level 1: **NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL**
