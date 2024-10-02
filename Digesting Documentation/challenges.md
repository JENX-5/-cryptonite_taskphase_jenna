# Digesting Documentation

## Challenge 1: Learning from Documentation
```bash
hacker@man~learning-from-documentation:~$ /challenge/challenge --giveflag
Correct argument! Here is your flag:
pwn.college{cExNePm9jVu_6qF07CRAu6o3wDt.dRjM5QDL0gTN0czW}
```
- Invoke the command with the given argument, didn't require any thought process.

## Challenge 2: Learning Complex Usage
```bash
hacker@man~learning-complex-usage:~$ /challenge/challenge --printfile /flag
Correct argument! Here is the /flag file:
pwn.college{kHvm7B9R0tdJmq4Sz3HDcIF_2S7.dVjM5QDL0gTN0czW}
```
- Giving an argument to another argument

## Challenge 3: Reading Manuals
```bash
hacker@man~reading-manuals:~$ man challenge

CHALLENGE(1)          Challenge Commands          CHALLENGE(1)

NAME
       /challenge/challenge - print the flag!

SYNOPSIS
       challenge OPTION

DESCRIPTION
       Output the flag when called with the right arguments.

       --fortune
              read a fortune

       --version
              output version information and exit

       --neshxm NUM
              print the flag if NUM is 400

AUTHOR
       Written by Zardus.

REPORTING BUGS
       The  repository for this dojo: <https://github.com/pwn‐
       college/linux-luminarium/>

SEE ALSO
       man(1) bash-builtins(7)
hacker@man~reading-manuals:~$ challenge --neshxm 400
ssh-entrypoint: challenge: command not found
hacker@man~reading-manuals:~$ /challenge/challenge --neshxm 400
Correct usage! Your flag: pwn.college{UnSDReshXxLHmXJjXkYavLio_IA.dRTM4QDL0gTN0czW}
```
- From the given manual, flag will be printed only when the --neshxm argument is used and the number argument is 400

## Challenge 4: Searching Manuals
```bash
hacker@man~searching-manuals:~$ man challenge
hacker@man~searching-manuals:~$ /challenge/challenge --arstu
Initializing...
Correct usage! Your flag: pwn.college{IN0s9i-1TWHHMMQzTmiur_svaat.dVTM4QDL0gTN0czW}
```
- In the manual, use / to search flag. After searching use 'n' to go to next search result and 'N' to go to previous one.
- When do the above process, you will get --arstu that gives the flag.

## Challenge 5: Searching for Manuals
```bash
hacker@man~searching-for-manuals:~$ man -k /challenge/challenge
lcjswxayjr (1)       - print the flag!
hacker@man~searching-for-manuals:~$ man lcjswxayjr

CHALLENGE(1)                                            Challenge Commands                                           CHALLENGE(1)

NAME
       /challenge/challenge - print the flag!

SYNOPSIS
       challenge OPTION

DESCRIPTION
       Output the flag when called with the right arguments.

       --fortune
              read a fortune

       --version
              output version information and exit

       --lcjswx NUM
              print the flag if NUM is 093

AUTHOR
       Written by Zardus.

REPORTING BUGS
       The repository for this dojo: <https://github.com/pwncollege/linux-luminarium/>

SEE ALSO
       man(1) bash-builtins(7)

pwn.college                                                  May 2024                                                CHALLENGE(1)
hacker@man~searching-for-manuals:~$ /challenge/challenge --lcjswx 093
Correct usage! Your flag: pwn.college{ElBUMc0CjswFxa9yjAr3IqU-f1B.dZTM4QDL0gTN0czW}
```
- Read the manual and found -k that gives a short manual description of the keyword.
- Then used the manual with argument -k to find out how to get the flag.

## Challenge 6: Helpful Programs
```bash
hacker@man~helpful-programs:~$ /challenge/challenge --help
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to give you the flag
hacker@man~helpful-programs:~$ /challenge/challenge -p
The secret value is: 40
hacker@man~helpful-programs:~$ /challenge/challenge -g 40
Correct usage! Your flag: pwn.college{QrLbZobVDUEyXT0BRtqsYnOeRYI.ddjM4QDL0gTN0czW}
```
- After reading the about the command, notice -p prints the needed value for -g to give the flag.
- First get the needed value and use it to get the flag

## Challenge 7: Help for Builtins
```bash
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!

    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "wYtILGb1".
hacker@man~help-for-builtins:~$ challenge --secret "wYtILGb1"
Correct! Here is your flag!
pwn.college{wYtILGb1gA-9i6wCQ29RbLdOQtm.dRTM5QDL0gTN0czW}
```
- Since challenge is a built-in command, we use help challenge instead of -h
- Getting the flag uses same logic as the previous question.
  
