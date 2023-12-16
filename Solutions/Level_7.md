#### *The password for the next level is stored in the file **data.txt** next to the word **millionth***

Use ssh command to connect to a remote host.

```bash
ssh bandit7@bandit.labs.overthewire.org -p 2220
```

Password: z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S

### Solution 
```bash
find / -name data.txt 2>/dev/null | xargs cat 2>/dev/null | grep millionth
```


Password for level 8: **TESKZC0XvTetK0S9xNwm25STk5iWrBvP**