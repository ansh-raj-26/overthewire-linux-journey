# Bandit Level 8 to 9

## Goal

The password for the next level is stored in the file data.txt and is the only line of text that occurs only once

---

## Level Information

- Username: 'bandit8'
- Host: 'bandit.labs.overthewire.org'
- Port: '2220'

---

## Command Used

ls
sort data.txt | uniq -u

## Process

1. Liste the files
2. Use sort command to sort the similars lines
3. Use uniq -u to find the line which occured only once


## What I Learned

- sort: organizes lines alphabetically
- uniq: filters duplicate lines
- uniq -u: shows only unique lines
- pipes (`|`): combine multiple commands together



## Important Concepts

- |: Passes output from one command into another

## Mistakes / Confusions

- Initially tried using uniq without sort
- Learned that uniq works properly only on sorted adjacent lines

------------

## Notes

|---|---|
| `grep "word" file` | search for word |
| `grep -i` | ignore uppercase/lowercase |
| `grep -n` | show matching line number |
| `grep -r` | recursive search |

