# Matching with []

```bash
hacker@globbing~matching-with-:~$ cd /challenge/files
hacker@globbing~matching-with-:/challenge/files$ /challenge/run file_[absh]
You got it! Here is your flag!
pwn.college{M-mKqryz5KeIxtRw1IzSBnd19AL.dNjM4QDL0gTN0czW}
```
- As the challenge instructed, first change the directory to /challenge/files
- Then to run the files using [], we put those characters which need to be matched with the given files.
- Here the files that need to be matched are file_a,file_b, file_s, file_h. So use file_[absh]
  
