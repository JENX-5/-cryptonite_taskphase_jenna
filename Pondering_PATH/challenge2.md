# Setting Path
- Instead of rewriting the values in PATH(which will still work). I appended the path for the win command so I can still use other commands if needed.
- Now the win command will work.
```bash
hacker@path~setting-path:~$ echo $PATH
/run/challenge/bin:/run/workspace/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
hacker@path~setting-path:~$ file=:/challenge/more_commands
hacker@path~setting-path:~$ PATH=$PATH$file
hacker@path~setting-path:~$ /challenge/run
Invoking 'win'....
Congratulations! You properly set the flag and 'win' has launched!
pwn.college{EXmCbTlLtbXud3WbwOxSndohQuH.dVzNyUDL0gTN0czW}
```
