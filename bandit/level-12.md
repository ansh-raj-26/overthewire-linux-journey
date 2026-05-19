# Bandit Level 12 to 13

## Goal

The password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work. Use mkdir with a hard to guess directory name. Or better, use the command “mktemp -d”. Then copy the datafile using cp, and rename it using mv.

----------

## Level Information

- Username: 'bandit12'
- Host: 'bandit.labs.overthewire.org'
- Port: '2220'

---

## Command Used

ls
mktemp -d

cd <pathname>

cp ~/data.txt .

xxd -r data.txt > data

file data

mv data data.gz
gunzip data.gz

mv data data.bz2
bunzip2 data.bz2

mv data data.tar
tar -xf data.tar

ls
file data5.bin
mv data5.bin data.tar
tar -xf data.tar

ls 
file data6.bin
mv data6.bin data.bz2
bunzip2 data.bz2

ls
file data8.bin
mv data8.bin data.gz
gunzip data.gz

file data

cat data

## Process

1. Created temporary directory using `mktemp -d`
2. Copied `data.txt` into working directory
3. Reversed hexdump using `xxd -r`
4. Used `file` repeatedly to identify compression type
5. Renamed files with correct extensions
6. Extracted compressed/archive files multiple times
7. Continued process until reaching ASCII text
8. Used `cat` to read final password

## What I Learned

- How hexdumps work
- Using `xxd` to reverse binary data
- Identifying unknown files using `file`
- Working with compression formats
- Extracting tar archives
- Recursive extraction workflow in Linux


## Important Concepts

Hexdump:A hexadecimal representation of binary data.

xxd: Used to create or reverse hexdumps. `(xxd -r file)`

file: Detects file type automatically.`file filename`

## Mistakes / Confusions

- Initially checked `data.txt` instead of extracted `data`
- Was ignoring the new file came after extraction.
- Thought data.txt was the final file.
- Realized `file` command is critical for identifying next step

------------

## Notes

|---|---|
| `xxd -r` | reverse hexdump |
| `file` | identify file type |
| `gunzip` | extract gzip |
| `bunzip2` | extract bzip2 |
| `tar -xf` | extract tar archive |
| `cat` | display file content |
