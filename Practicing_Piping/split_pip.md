# Split Piping Stderr and Stdout
## Challenge 11
- Redirect the stderr using file descriptor 2> as input using >(/challenge/the).
- Then use pip | for /challenge/planet since anyway only stdout is passed in pip.
- Or you can > > again.
  
```bash
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack 2> >( /challenge/the ) | /challenge/planet
Congratulations, you have learned a redirection technique that even experts
struggle with! Here is your flag:
pwn.college{U0jbrCOBWfXaa9HIkcvGlCwS3tP.dFDNwYDL0gTN0czW}
```
> Alternate Way
```bash
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack 2> >( /challenge/the) > >(/challenge/planet)
Congratulations, you have learned a redirection technique that even experts
struggle with! Here is your flag:
pwn.college{U0jbrCOBWfXaa9HIkcvGlCwS3tP.dFDNwYDL0gTN0czW}
```
## References
- [Link](https://superuser.com/questions/517256/obtain-both-merged-and-separated-stdout-and-stderr)
  
