# Bandit Level 10 to 11

## Goal

The password for the next level is stored in the file data.txt and is the only line of text that occurs only once

---
nvim
## Level Information

- Username: 'bandit8'
- Host: 'bandit.labs.overthewire.org'tre
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
# Bandit Level 8 to 9

## Goal

The password for the next level is stored in the file data.txt and is the only line of text that occurs only once

---
nvim
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

- How to use base64 to decode the binary values
- How we can conver the readable text to base64
- But anyone can decode it easily 
- = is generally for padding



## Important Concepts

- `base64`: is an encoding method used to convert data into readable text format.
- `-d`: used for decoding

## Mistakes / Confusions

- What is the format of running base64 command
- I used `echo<filedata>|base64 -d` to decode
- I would have use `base64 -d <filebame>`

------------

## Notes

|---|---|
| `base64` | encode data |
| `base64 -d` | decode data |
| `echo` | print text |
| `|` | combine commands |

