# Mixing Globs

```bash
hacker@globbing~mixing-globs:~$ cd /challenge/files
hacker@globbing~mixing-globs:/challenge/files$ ls
amazing      fantastic   kind        pwning     uplifting   zesty
beautiful    great       laughing    queenly    victorious
challenging  happy       magical     radiant    wonderful
delightful   incredible  nice        splendid   xenial
educational  jovial      optimistic  thrilling  youthful
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run [cep]*
You got it! Here is your flag!
pwn.college{QNMPbtj97w0shyPR0dKsXS7SAGJ.dVjM4QDL0gTN0czW}
```
- We have to ensure that the given argument should be less than 6 characters.
- Notice in all the files in /challenge/files, no two files start with the same alphabet.
- So we can use [] and add all the alphabets of the words to match that is 'educational','pwning','challenging'.
- so \[epc]* will match with any file that begins with e, p and c with * being the wildcard.
