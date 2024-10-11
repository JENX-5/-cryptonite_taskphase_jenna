# Fun with Group Names
- Use id to find the group your in.
- Here the group is grp16432.
- Using chgrp change the ownership to the given group and read the contents of /flag using cat.
```bash
hacker@permissions~fun-with-groups-names:~$ id
uid=1000(hacker) gid=1000(grp16432) groups=1000(grp16432)
hacker@permissions~fun-with-groups-names:~$ ls -l / | grep flag
-r--r-----    1 root root   58 Oct 11 17:04 flag
hacker@permissions~fun-with-groups-names:~$ chgrp grp16432 /flag
hacker@permissions~fun-with-groups-names:~$ cat /flag
pwn.college{cpovW6aACbGsWm_LqYD3y3IElz8.dJzNyUDL0gTN0czW}
```
