# Level 3
# Description
The password for the next level is stored in a hidden file in the inhere directory.

# Solution
- Use find command to find all directories having inhere.

```bash
bandit3@bandit:~$ find inhere
inhere
inhere/...Hiding-From-You
bandit3@bandit:~$ cat inhere/...Hiding-From-You
2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ
```
