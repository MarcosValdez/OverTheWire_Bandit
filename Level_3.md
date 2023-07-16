#### *The password for the next level is stored in a hidden file in the **inhere** directory.*

Use ssh command to connect to a remote host.

```bash
ssh bandit3@bandit.labs.overthewire.org -p 2220
```

Password: aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG

### Solution 1
```bash
cd inhere; ls -a; cat .hidden
```
*The flag `-a` do not ignore entries starting with. One way to execute several commands at the same time is to separate them with `;` in this way the commands will be executed sequentially regardless of whether one of them fails.*

### Solution 2
```bash
find . -name .hidden | xargs cat
```
*xargs (e**x**tended **arg**ument**s**), some commands like grep can accept input as parameters, but some commands accepts arguments, this is place where xargs came into picture. Xargs reads items from the standard input.*

Password for level 4: 2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe