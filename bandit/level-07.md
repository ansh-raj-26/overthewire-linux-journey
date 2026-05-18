# Bandit Level 6 to 7

## Goal

The password for the next level is stored somewhere on the server and has all of the following properties:

owned by user bandit7
owned by group bandit6
33 bytes in size

---

## Level Information

- Username: 'bandit6'
- Host: 'bandit.labs.overthewire.org'
- Port: '2220'

---

## Command Used

ls -a
find / -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null
cat <filepath>

## Process

1. Opened terminal
2. Used SSH command
3. Entered password provided by OverTheWire
4. Successfully logged into remote Linux machine
5. List the file
6. To find hidden file run ls -a command.
7. Use find command and write the properties(user,group, etc)
8. USe cat with the comple file path shown

## What I Learned

- How to avoid permisiion denied error 
- How to use 2>/dev/null

## Important Concepts

- 2>/dev/null: 2 = stderr (errors),2 = stderr (errors), 2 = stderr (errors) 

## Mistakes / Confusions

- Forgot to give the / after filec
- How to get permisiion 
------------

## Notes

| Part             | Meaning                |
| ---------------- | ---------------------- |
| `find /`         | search entire system   |
| `-type f`        | only files             |
| `-user bandit7`  | owned by user bandit7  |
| `-group bandit6` | owned by group bandit6 |
| `-size 33c`      | exactly 33 bytes       |
| `2>/dev/null`    | hide permission errors |

