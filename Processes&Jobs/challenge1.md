# LISTING PROCESSES
- To see all the processes running in an environment we use ps.
- We can use two arguments with -es and aux, they give almost the same results(with some differences in the output).
- In the challenge the flag is in a program which is running in the background. So find the processes running , using ps aux.
- Then find the flag by executing the program.(Here the file was in /challenge/15718-run-30108)
```bash
hacker@processes~listing-processes:~$ ps aux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.1  0.0   1056   640 ?        Ss   17:20   0:00 /sbin/docker-init -- /nix/var/nix/profiles/default/bi
root           7  0.0  0.0   5052  2560 ?        S    17:20   0:00 /run/dojo/bin/sleep 6h
root          68  0.0  0.0   4132  2560 ?        S    17:20   0:00 /challenge/15718-run-30108
root          72  0.0  0.0   2744  1600 ?        S    17:20   0:00 sleep 6h
hacker        73  0.2  0.0   5372  3840 pts/0    Ss   17:21   0:00 /run/dojo/bin/ssh-entrypoint
hacker        90  0.0  0.0   7868  3520 pts/0    R+   17:21   0:00 ps aux
hacker@processes~listing-processes:~$ /challenge/15718-run-30108
Yahaha, you found me! Here is your flag:
pwn.college{kJp9TJI9tszwOPid3B7NqgJZ9iT.dhzM4QDL0gTN0czW}
Now I will sleep for a while (so that you could find me with 'ps').
```
