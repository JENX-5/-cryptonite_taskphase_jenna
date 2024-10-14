# Cracking Passwords
- Use john(John The Ripper tool) [file] to get all the passwords.
- Can use the argument --show to show all the passwords of the users.
- Use the password and get the flag.
```bash
hacker@users~cracking-passwords:~$ john /challenge/shadow-leak
Created directory: /home/hacker/.john
Loaded 1 password hash (crypt, generic crypt(3) [?/64])
Press 'q' or Ctrl-C to abort, almost any other key for status
0g 0:00:00:15 0% 2/3 0g/s 285.2p/s 285.2c/s 285.2C/s deedee..grizzly
aardvark         (zardus)
1g 0:00:00:20 100% 2/3 0.04873g/s 283.7p/s 283.7c/s 283.7C/s Johnson..buzz
Use the "--show" option to display all of the cracked passwords reliably
Session completed
hacker@users~cracking-passwords:~$ su zardus
Password:
zardus@users~cracking-passwords:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{wstKSqXLnXBFfw7fZRNaOSNvYyX.ddTN0UDL0gTN0czW}
```
