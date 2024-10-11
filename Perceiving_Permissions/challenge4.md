# Changing Permissions
- The permission to read the contents of the flag is set only to the root user.
- So we can change it my using chmod.
- Used chmod go+r (**g**roup,**o**thers) to give permission to other users to read the /flag file.
- Technically this isn't possible if the you don't have permission to write in the file but they made it possible for the challenge
 
```bash
hacker@permissions~changing-permissions:~$ ls -l /flag
-r-------- 1 root root 58 Oct 11 17:16 /flag
hacker@permissions~changing-permissions:~$ chmod go+r *
hacker@permissions~changing-permissions:~$ ls -l /flag
-r--r--r-- 1 root root 58 Oct 11 17:16 /flag
hacker@permissions~changing-permissions:~$ cat /flag
pwn.college{kXo_9EMEFVW-gfgTD5eyHeYKllz.dNzNyUDL0gTN0czW}
```
