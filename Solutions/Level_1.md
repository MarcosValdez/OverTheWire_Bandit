*The password for the next level is stored in a file called **-** located in the home directory*

Use ssh command to connect to a remote host.
```bash
ssh bandit1@bandit.labs.overthewire.org -p 2220
```

Password: NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL

### Solution 1
```bash
cat ./-
```
*"When `cat` sees the string `-` as a filename, it treats it as a synonym for stdin. To get around this, you need to alter the string that `cat` sees in such a way that it still refers to a file called `-`. The usual way of doing this is to prefix the filename with a path - `./-`, or `/home/Tim/-`."* [Reference](https://unix.stackexchange.com/questions/16357/usage-of-dash-in-place-of-a-filename)

### Solution 2
```bash
cat $(pwd)/-
```
*"It's called command substitution (posix specification) and it invokes a subshell. The command in the braces of `$()` or between the backticks (`` `…` ``) is executed in a subshell and the output is then placed in the original command."* [Reference](https://unix.stackexchange.com/questions/147420/what-is-in-a-command)

Password for level 2: **rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi**
