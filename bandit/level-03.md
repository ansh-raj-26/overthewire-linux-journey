# Bandit Level 2 to 3

## Goal

The password for the next level was stored in a file called --spaces in this filename--



---

## Level Information

- Username: 'bandit2'
- Host: 'bandit.labs.overthewire.org'
- Port: '2220'

---

## Command Used

cat ./--spaces\ in\ this\ filename--

## Process

1. Opened terminal
2. Used SSH command
3. Entered password provided by OverTheWire
4. Successfully logged into remote Linux machine
5. List the file
6. For expression file we have to use cat with ./ as the file staring name is in some symboles
7. Then for the spaces in the filename we have to add "\" everywhere necessary.
8. Then linux recognize it as single file name.

## What I Learned

- How to open a file which has expression
- How to make linux undersatnd to ignore the sapces between the file name.

## Important Concepts

- cat./: cat is for reading the file and, "./" is used for opening a symbolic files
- \ : This is used in between the spaces given in the file name whihc escapes the spaces and make the machine unders      tand as a single file name. 

## Mistakes / Confusions

- First i thought we just have to ./ for the initial symbol only and nothing else
- When to add the backshlash like where to add it at the end also start aslo where?


## Notes

--------------------------------------------------------------------------------------------------------------------
