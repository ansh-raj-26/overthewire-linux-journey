# Bandit Level 13 to 14

## Goal

Use the SSH private key provided in `sshkey.private` to log into the `bandit14` account.

----------

## Level Information

- Username: 'bandit13'
- Host: 'bandit.labs.overthewire.org'
- Port: '2220'

---

## Command Used

scp -P 2220 bandit13@bandit.labs.overthewire.org:~/sshkey.private ./bandit14.key

chmod 600 bandit14.key

ssh -i bandit14.key -p 2220 bandit14@bandit.labs.overthewire.org

## Process

1. Copied the private SSH key from the remote Bandit server to local machine using `scp`
2. Secured the key using `chmod 600`
3. Logged into the `bandit14` account using key-based authentication
4. Successfully accessed the next level

## What I Learned

- What is `scp`
- How to securely copy files using `scp`
- SSH can authenticate using private keys instead of passwords
- SSH private keys require strict permissions
- `chmod 600` is standard for private key security
- How to get sshkey.private 



## Important Concepts

scp: Used to securely transfer files over SSH.
`:~/sshkey.private`  remote file path |
`./bandit14.key` save locally with this name


file: Detects file type automatically.`file filename`

## Mistakes / Confusions

- Initially checked `data.txt` instead of extracted `data`
- Was ignoring the new file came after extraction.
- Thought data.txt was the final file.
- Realized `file` command is critical for identifying next step

------------

## Notes

| Command | Action |
|---|---|
| `scp` | copy files over SSH |
| `ssh -i` | use private key authentication |
| `chmod 600` | secure private key |
| `-p 2220` | custom SSH port || Command | Action |

| Value | Permission |
|---|---|
| `6` | read + write |
| `0` | no permissions |
| `0` | no permissions |

