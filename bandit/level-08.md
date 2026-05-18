# Bandit Level 7 to 8

## Goal

Find the password stored in data.txt next to the word millionth.

---

## Level Information

- Username: 'bandit7'
- Host: 'bandit.labs.overthewire.org'
- Port: '2220'

---

## Command Used

ls
cat data.txt
grep "millionth" data.txt

## Process

1. Liste the files
2. Tried veiwing the file with cat command
3. As the file was large used grep command for the specific word.


## What I Learned

- grep: searches text patterns inside files
- Searching is more efficient than reading huge files manually
- Linux commands can be combined to filter useful information quickly

## Important Concepts

- grep: Used for searchinh the text pattern

## Mistakes / Confusions

- Initially tried reading entire file with cat
- Learned that grep is much faster for searching specific text 

------------

## Notes

|---|---|
| `grep "word" file` | search for word |
| `grep -i` | ignore uppercase/lowercase |
| `grep -n` | show matching line number |
| `grep -r` | recursive search |

