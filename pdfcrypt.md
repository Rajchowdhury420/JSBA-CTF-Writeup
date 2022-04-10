```bash
$ perl pdf2john.pl /mnt/d/Downloads/encrypted.pdf > pdf.hash
```
```bash
$ john pdf.hash --wordlist=/usr/share/wordlists/rockyou.txt
Using default input encoding: UTF-8
Loaded 1 password hash (PDF [MD5 SHA2 RC4/AES 32/64])
Cost 1 (revision) is 4 for all loaded hashes
Will run 6 OpenMP threads
Press 'q' or Ctrl-C to abort, almost any other key for status
hacked           (/root/CTF/encrypted.pdf)
1g 0:00:00:00 DONE (2022-02-24 20:07) 3.448g/s 180744p/s 180744c/s 180744C/s lights1..gummybear1
Use the "--show --format=PDF" options to display all of the cracked passwords reliably
Session completed
```
#### When I opened the pdf with the password I found, I found the flag
```bash
flag {kramer_the_best_hacker_ever}
```
