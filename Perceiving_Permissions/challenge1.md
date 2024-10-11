# Changing File Ownership
- We change the ownership of the file by using chown \[username] \[file].
- Using ls -l | grep flag to show that the ownership was initially root then changed to user hacker.
```bash
hacker@permissions~changing-file-ownership:~$ ls -l / | grep flag
-r--------    1 root root   58 Oct 11 16:46 flag
hacker@permissions~changing-file-ownership:~$ chown hacker /flag
hacker@permissions~changing-file-ownership:~$ ls -l / | grep flag
-r--------    1 hacker root   58 Oct 11 16:46 flag
hacker@permissions~changing-file-ownership:~$ cat /flag
pwn.college{YBkwuXG6Rg8ldjwJhNh5da4tADR.dFTM2QDL0gTN0czW}
```
