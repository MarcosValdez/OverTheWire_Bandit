#### *The password for the next level is stored in a file somewhere under the **inhere** directory and has all of the following properties:*
- human-readable
- 1033 bytes in size
- not executable

Use ssh command to connect to a remote host.

```bash
ssh bandit5@bandit.labs.overthewire.org -p 2220
```

Password: lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR

### Solution 
```bash
find . -type f -readable -size 1033c | xargs cat
```
*Be located in the directory `inhere`*. 

Password for level 6: **P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU**