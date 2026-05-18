# Bandit Level 9 to 10

## Goal

The password for the next level is stored in the file data.txt in one of the few human-readable strings, preceded by several ‘=’ characters.

---

## Level Information

- Username: 'bandit9'
- Host: 'bandit.labs.overthewire.org'
- Port: '2220'

---

## Command Used

ls
strings data.txt
strings data.txt | grep "=="

## Process

1. Liste the files
2. Try to view the file
3. Use `string`command to view the readable format 
4. The key precede with the `=` so we use `grep` command.

## What I Learned

- strings: to convert non readbale data to readable data 
- grep: can filter useful data 
- binary file may have human readable text also 
- pipes (`|`): combine multiple commands together



## Important Concepts

- `grep "=="` sreaches for matching text pattern
- `strings <filename>` show the readable data in binary files 

## Mistakes / Confusions

- Which command to run grep or string
- Binary files and not easy to read the data 
- fomat of string command 
- first used string -d <filename>

---------------------------------------------------------------------------------------------

