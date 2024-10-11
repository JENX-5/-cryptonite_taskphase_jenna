# Group and Files
- Here instead of changing the ownership user, we changed the group that owns the file.
- To do that use chgrp \[user] \[filename] and then you can access the flag file
```bash
hacker@permissions~groups-and-files:~$ ls -l / | grep flag
-r--r-----    1 root root   58 Oct 11 16:58 flag
hacker@permissions~groups-and-files:~$ chgrp hacker /flag
hacker@permissions~groups-and-files:~$ ls -l / | grep flag
-r--r-----    1 root hacker   58 Oct 11 16:58 flag
hacker@permissions~groups-and-files:~$ cat /flag
pwn.college{stkJnWibg2di1uai71RtKu4Y0eV.dFzNyUDL0gTN0czW}
```
