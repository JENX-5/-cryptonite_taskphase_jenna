# LEVEL 4
# Description
The password for the next level is stored in the only human-readable file in the inhere directory. 
Tip: if your terminal is messed up, try the “reset” command.

# Solution
- Use file to find the type of file. Read the contents of ASCII text file.
```bash
bandit4@bandit:~$ ls inhere
-file00  -file02  -file04  -file06  -file08
-file01  -file03  -file05  -file07  -file09
bandit4@bandit:~$ file inhere/-file0?
inhere/-file00: data
inhere/-file01: data
inhere/-file02: data
inhere/-file03: data
inhere/-file04: data
inhere/-file05: data
inhere/-file06: data
inhere/-file07: ASCII text
inhere/-file08: data
inhere/-file09: data
bandit4@bandit:~$ cat inhere/-file07
4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
```
