#### *The password for the next level is stored **somewhere on the server** and has all of the following properties:*
- owned by user bandit7
- owned by group bandit6
- 33 bytes in size

Use ssh command to connect to a remote host.

```bash
ssh bandit6@bandit.labs.overthewire.org -p 2220
```

Password: P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU

### Solution 
```bash
find / -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null | xargs cat
```
*2>/dev/null redirects error messages to null so that they do not show on stdout.*

Password for level 7: **z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S**