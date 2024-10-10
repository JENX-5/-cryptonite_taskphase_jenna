# Suspending Processes
- Instead of interrupting a process, you can just suspend it by Ctrl-Z.
- So run /challenge/run then suspend and run it again. So there are two copies of the same file running.
  
```bash
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root          83      65  0 17:49 pts/0    00:00:00 bash /challenge/run
root          85      83  0 17:49 pts/0    00:00:00 ps -f

I don't see a second me!

To pass this level, you need to suspend me and launch me again! You can
background me with Ctrl-Z or, if you're not ready to do that for whatever
reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root          83      65  0 17:49 pts/0    00:00:00 bash /challenge/run
root          90      65  0 17:49 pts/0    00:00:00 bash /challenge/run
root          92      90  0 17:49 pts/0    00:00:00 ps -f

Yay, I found another version of me! Here is the flag:
pwn.college{UNod7j-t3Ny3RPGy3brbx-f8t5x.dVDN4QDL0gTN0czW}
```
