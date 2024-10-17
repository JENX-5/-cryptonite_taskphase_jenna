# Adding Commands
- First add then needed commands(here just cat /fal to win.
- Now we need to add the path of win to the PATH.
- Find the directory you stored win in(here it was in the current working directory).
- Add the path of win to PATH.
- Now run /challenge/run. Notice it says permission denied. That's because we didn't give permissions to execute the file.
- Change the permission to be able to execute the file and run the file again.
```bash
hacker@path~adding-commands:~$ echo "cat /flag" > win
hacker@path~adding-commands:~$ pwd
/home/hacker
hacker@path~adding-commands:~$ PATH=$PATH:/home/hacker
hacker@path~adding-commands:~$ /challenge/run
Invoking 'win'....
/challenge/run: line 4: /home/hacker/win: Permission denied
It looks like that did not work... Did you set PATH correctly?
hacker@path~adding-commands:~$ chmod ug+x /home/hacker/win
hacker@path~adding-commands:~$ /challenge/run
Invoking 'win'....
pwn.college{4PIccDwPRnalRC4VtO7wWCRWREO.dZzNyUDL0gTN0czW}
```
