# Redirecting Inputs
## Challenge 5
- First redirect output college to file PWN using >
- Then redirect the input of PWN to /challenge/run using <
```bash
hacker@piping~redirecting-input:~$ echo COLLEGE > PWN
hacker@piping~redirecting-input:~$ /challenge/run < PWN
Reading from standard input...
Correct! You have redirected the PWN file into my standard input, and I read
the value 'COLLEGE' out of it!
Here is your flag:
pwn.college{oV-TkF5JWTqaj99mNfmO42XTqyt.dBzN1QDL0gTN0czW}
```
