```bash
❯ binwalk -D='.*' a_friend.zip

DECIMAL       HEXADECIMAL     DESCRIPTION
--------------------------------------------------------------------------------
0             0x0             Zip archive data, at least v2.0 to extract, compressed size: 12250, uncompressed size: 24626, name: a friend.docx
12404         0x3074          End of Zip archive, footer length: 22
12426         0x308A          PNG image, 5312 x 2988, 8-bit/color RGB, non-interlaced
15889         0x3E11          Zlib compressed data, default compression

```
so we can see 0x308A is a png , lets see what it is

![](https://raw.githubusercontent.com/Rajchowdhury420/temp-files-for-writeup/main/bingo.png)
Bingo we got the flag !
