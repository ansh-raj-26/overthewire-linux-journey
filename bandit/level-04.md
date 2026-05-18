# Bandit Level 3 to 4

## Goal

I had to find the hidden file inside a director

---

## Level Information

- Username: 'bandit3'
- Host: 'bandit.labs.overthewire.org'
- Port: '2220'

---

## Command Used

ls
cd inhere
ls -a
cat ./.  ..  ...Hiding-From-You

## Process

1. Opened terminal
2. Used SSH command
3. Entered password provided by OverTheWire
4. Successfully logged into remote Linux machine
5. List the file
6. To find hidden file run ls -a command.
7. For expression file we have to use cat with ./<filename>

## What I Learned

- How to open a file which is hidden

## Important Concepts

- ls -a: Shows hidden files.

## Mistakes / Confusions

------------

## Notes

Command 	Action
ls -l	Long listing format: Displays detailed info like permissions, owner, size, and modification date.
ls -a	Show hidden files: Includes files that start with a dot (.), which are usually hidden by default.
ls -lh	Human-readable: Used with -l to show file sizes in KB, MB, or GB instead of bytes.
ls -t	Sort by time: Lists items based on when they were last modified (newest first).
ls -R	Recursive listing: Shows the contents of all subdirectories within the target folder.
