# Bandit Level 4 to 5

## Goal

The password is stored in a human readable file

---

## Level Information

- Username: 'bandit4'
- Host: 'bandit.labs.overthewire.org'
- Port: '2220'

---

## Command Used

ls
cd inhere
file ./*
cat ./-file07

## Process

1. Opened terminal
2. Used SSH command
3. Entered password provided by OverTheWire
4. Successfully logged into remote Linux machine
5. List the file
6. To find human readble file type file ./*
7. The ASCII text can be read so run cat ./-file07


## What I Learned

- How to find a types of file
- How to know which file readable

## Important Concepts

- file ./*: Lets you know the file type of all the listed files.

## Mistakes / Confusions

- Which command to use i was using find,grep(dont know why..).
- Runnning something like grep type -f
------------

## Notes

---------------------------------------------------------------------------------------------
