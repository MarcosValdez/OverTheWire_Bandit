#### *The password for the next level is stored in the only human-readable file in the **inhere** directory. Tip: if your terminal is messed up, try the “reset” command.*

Use ssh command to connect to a remote host.

```bash
ssh bandit4@bandit.labs.overthewire.org -p 2220
```

Password: 2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe

### Solution 1
```bash
file ./*; cat ./-file07
```
*Be located in the directory `inhere`*. This command return a list, where it shows us `inhere/-file07: ASCII text`.

### Solution 2
```bash
find . -name '-file07' | xargs cat
```

Password for level 5: **lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR**