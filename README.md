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
