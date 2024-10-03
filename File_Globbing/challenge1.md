# Matching with *

- We are supposed to change the directory while using only 4 characters
- Using File Globbing we can use * , ch* matches with any entry that begins with ch
- So the directory gets changed to challenge.
  
```bash
hacker@globbing~matching-with-:~$ cd /ch*
hacker@globbing~matching-with-:/challenge$ /challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{4cxmAjRlRO_HX0gcUf3MKHyhjni.dFjM4QDL0gTN0czW}
hacker@globbing~matching-with-:/challenge$
```

