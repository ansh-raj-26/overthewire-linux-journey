# Bandit Level 0

## Goal

 I had to connect Bandit using SSH.

---

## Level Information

- Username: 'bandit0'
- Host: 'bandit.labs.overthewire.org'
- Port: '2220'

---

## Command Used


ssh bandit0@bandit.labs.overthewire.org -p 2220



## Process

1. Opened terminal
2. Used SSH command
3. Entered password provided by OverTheWire
4. Successfully logged into remote Linux machine

---

## What I Learned

- Basic SSH login
- How to connect server to the terminal using SSH commands
- Structure of SSH commands

---

## Important Concepts

### SSH

SSH (Secure Shell) is used to securely connect to remote systems through terminal.

Basic syntax:


ssh username@host


Custom port syntax:


ssh username@host -p PORT


## Mistakes / Confusions

- Initially was confused where to write username and host.
- What is the format to write a SSH command

## Useful Commands

Check current logged in user:

```bash
whoami
```

Check current directory:

```bash
pwd
```

List files:

```bash
ls
```

##Steps:

- Check which directory you are in.
- Just write the ssh command.
- Enter the password.
- Done
