# Bandit Level 0 to 1

## Goal

The password for the next level is stored in a file called readme located in the home directory. Use this password to log into bandit1 using SSH

---

## Level Information

- Username: 'bandit1'
- Host: 'bandit.labs.overthewire.org'
- Port: '2220'

---

## Command Used


ssh bandit0@bandit.labs.overthewire.org -p 2220
ls
cat readme


## Process

1. Opened terminal
2. Used SSH command
3. Entered password provided by OverTheWire
4. Successfully logged into remote Linux machine
5. Now list the file and using cat command i retrived the password

---

## What I Learned

- Commands like how i can list the files in the directory i amd wroking on 
- how to see the readable data in the file in terminal itself.

---

## Important Concepts

### SSH

ls: List the content of the directory 
cat: used to display text files directly in the terminal 

## Mistakes / Confusions

- how do i find i password in the given file 
- which command to use for opening/reading the file to find the password 

## Steps:

- Check the directory 
- List content 
- Display the file provided
- Done

