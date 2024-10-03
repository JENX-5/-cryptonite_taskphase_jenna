# Exclusionary Globbing
```bash
hacker@globbing~exclusionary-globbing:~$ cd /challenge/files
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run [!pwn]*
You got it! Here is your flag!
pwn.college{M5lrbcRX9pmsJYYbXK5uBwp7eZj.dZjM4QDL0gTN0czW}
```
- We need to match files which don't begin with p,w,n and do it within 8 arguments.
- [!a] is used when you want files that dont start with the letter a. So for the given challenge\
  [!pwn] should be used.
- Also the files can end with anything, therefore we add * at the end.
- The final answer should be [!pwn]*  which is less than 8 characters.
