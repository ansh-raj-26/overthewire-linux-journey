# Bandit Level 5 to 6

## Goal

Had to find a file with these properties human-readable, 1033 bytes in size, not executable

---

## Level Information

- Username: 'bandit5'
- Host: 'bandit.labs.overthewire.org'
- Port: '2220'

---

## Command Used

ls
cd inhere
ls
find type -f -size 1033c
cat ./maybehere07/.file2

## Process

1. Opened terminal
2. Used SSH command
3. Entered password provided by OverTheWire
4. Successfully logged into remote Linux machine
5. List the file
6. Use find command with type and specify the size 
7. By cat command read the file.

## What I Learned

- How to find the specific type of file user/i want to obtain
- How to use find command

## Important Concepts

-| Part          | Meaning                          |
| ------------- | -------------------------------- |
| `find`        | search for files/directories     |
| `-type f`     | only look for files (`f` = file) |
| `-size 1033c` | file size exactly 1033 bytes     |
| `c`           | bytes/characters                 |


## Mistakes / Confusions

- Which command to use 
- Writing type -f instead of -type f

------------

## Notes

--------------------------------------------------------------------------------------------
