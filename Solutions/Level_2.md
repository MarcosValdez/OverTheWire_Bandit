### *The password for the next level is stored in a file called **spaces in this filename** located in the home directory*

Use ssh command to connect to a remote host.

```bash
ssh bandit2@bandit.labs.overthewire.org -p 2220
```

Password: rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi

### Solution 1
```bash
cat 'spaces in this filename'
```
*You can't directly write spaces in the file name because if you have a space in the file name it will try to read multiple files.*

### Solution 2
```bash
cat spaces\ in\ this\ filename
```
*A backslash escapes the next character from being interpreted by the shell. If the next character after the backslash is a newline character, then that newline will not be interpreted as the end of the command by the shell.*
*Use `\` before the space in the file name to show that you mean space character.*

Password for level 3: **aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG**
