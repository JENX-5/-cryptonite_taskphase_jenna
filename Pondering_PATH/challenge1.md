# The Path Variable
- PATH stores all the directory paths.
- By setting its value to nothing. It won't be able to locate the where the command is stored.

```bash
hacker@path~the-path-variable:~$ PATH=""
hacker@path~the-path-variable:~$ /challenge/run
Trying to remove /flag...
/challenge/run: line 4: rm: No such file or directory
The flag is still there! I might as well give it to you!
pwn.college{4h2U3jWF82l0uOgCLDV0Xn6Qqgf.dZzNwUDL0gTN0czW}
```
