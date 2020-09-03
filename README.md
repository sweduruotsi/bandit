# bandit

## Level 0

The goal of this level is for you to log into the game using SSH. The host to which you need to connect is bandit.labs.overthewire.org, on port 2220. The username is bandit0 and the password is bandit0. Once logged in, go to the Level 1 page to find out how to beat Level 1.

ssh bandit.labs.overthewire.org -p2220 -l bandit0

## Level 1

The password for the next level is stored in a file called readme located in the home directory. Use this password to log into bandit1 using SSH. Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.
Commands you may need to solve this level

ls, cd, cat, file, du, find

ls -la
cat readme
boJ9jbbUNNfktd78OOpsqOltutMc3MY1


## Level 2

The password for the next level is stored in a file called - located in the home directory
Commands you may need to solve this level

ls, cd, cat, file, du, find
Helpful Reading Material

    Google Search for “dashed filename”
    Advanced Bash-scripting Guide - Chapter 3 - Special Characters
    
cat < - 
CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9

## Level 3

The password for the next level is stored in a file called spaces in this filename located in the home directory
Commands you may need to solve this level

ls, cd, cat, file, du, find
Helpful Reading Material

    Google Search for “spaces in filename”

cat "spaces in this filename"
UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK

## level 4

The password for the next level is stored in a hidden file in the inhere directory.
Commands you may need to solve this level

ls, cd, cat, file, du, find

cat .hidden
pIwrPrtPN36QITSp3EQaw936yaFoFgAB

## level 5

The password for the next level is stored in the only human-readable file in the inhere directory. Tip: if your terminal is messed up, try the “reset” command.
Commands you may need to solve this level

ls, cd, cat, file, du, find

cat < -file07
koReBOKuIDDepwhWk7jZC0RTdopnAYKh

## level 6

The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:

    human-readable
    1033 bytes in size
    not executable

Commands you may need to solve this level

ls, cd, cat, file, du, find

find . * -size 1033c
cat maybehere07/.file2
DXjZPULLxYr17uwoI01bNLQbtFemEgo7

# level 7

The password for the next level is stored somewhere on the server and has all of the following properties:

    owned by user bandit7
    owned by group bandit6
    33 bytes in size

find . * -size 33c -group bandit6 -user bandit7

cat ./var/lib/dpkg/info/bandit7.password
HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs

## level 8

The password for the next level is stored in the file data.txt next to the word millionth

ssh bandit.labs.overthewire.org -p2220 -l bandit7
HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs

strings data.txt | grep milliont
millionth	cvX2JJa4CFALtqS87jk27qwqGhBM9plV

## level 9

The password for the next level is stored in the file data.txt and is the only line of text that occurs only once
Commands you may need to solve this level

grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd
Helpful Reading Material

    Piping and Redirection

sort data.txt | uniq -c
UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR

## level 10

The password for the next level is stored in the file data.txt in one of the few human-readable strings, preceded by several ‘=’ characters.
Commands you may need to solve this level

grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

ssh bandit.labs.overthewire.org -p2220 -l bandit9

strings data.txt | grep ===
truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk


## level 11
The password for the next level is stored in the file data.txt, which contains base64 encoded data
Commands you may need to solve this level

grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

base64 -d data.txt
IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR

## level 12 

The password for the next level is stored in the file data.txt, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions
Commands you may need to solve this level

grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd
Helpful Reading Material

    Rot13 on Wikipedia

cat data.txt
Gur cnffjbeq vf 5Gr8L4qetPEsPk8htqjhRK8XSP6x2RHh
echo Gur cnffjbeq vf 5Gr8L4qetPEsPk8htqjhRK8XSP6x2RHh | tr 'A-Za-z' 'N-ZA-Mn-za-m'
The password is 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu


