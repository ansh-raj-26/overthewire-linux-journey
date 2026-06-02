# Bandit Level 14 to 15

## Goal

The password for the next level can be retrieved by submitting the password of the current level to port 30000 on localhos.
----------

## Level Information

- Username: 'bandit14'
- Host: 'bandit.labs.overthewire.org'
- Port: '2220'

---

## Command Used

cat /etc/bandit_pass/bandit14

nc localhost 30000

## Process

1. Read the current password stored in:/etc/bandit_pass/bandit14
2. Connected to the service listening on port 30000 using: nc localhost 30000
3. Submitted the password obtained from the previous step.
4. The service verified the password.
5. Received the password for bandit15.

## What I Learned

- Basic client-server communication
- How TCP ports are used
- What localhost means
- Using Netcat (nc) to connect to services
- Sending data through a TCP connection
- Using pipes (|) to automate command input

## Important Concepts

- Netcat (nc): A networking utility used for:

Opening TCP connections
Sending data
Receiving data
Testing services

Syntax:

nc host port

Example:

nc localhost 30000

## Mistakes / Confusions

- Initially expected the password to be stored in a file.
- Forgot that the challenge required sending the password to a network service.
- Confused localhost with a remote server.
- Did not realize Netcat waits silently for input after connecting.

------------

## Notes

| Command                                 | Purpose                          |
| --------------------------------------- | -------------------------------- |
| `cat /etc/bandit_pass/bandit14`         | Read current password            |
| `nc localhost 30000`                    | Connect to service               |
| `echo "PASSWORD" \| nc localhost 30000` | Send password automatically      |
| `localhost`                             | Current machine (127.0.0.1)      |
| `30000`                                 | Service port used in this level  |
| `nc`                                    | Netcat networking utility        |
| `\|`                                    | Pipe output into another command |

