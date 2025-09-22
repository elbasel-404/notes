# Linux notes

## This appends text to a file

echo Hello World >> peanuts.txt

## This overwrites the file

echo Hello World > peanuts.txt

## This redirects stdin instead of the terminal input to a file

cat < peanuts.txt > banana.tx

## this prints out an erro to the screen

ls /fake/directory > peanuts.txt

## stdin = 1

## stdout = 2

## stderr = 3

tail -f /var/log/syslog

ls /somedir | grep '.txt$'

## Regular expressions

tex="sally sells seashells

by the seashore"

^by
would match the line "by the seashore"

seashore$
would match the line "by the seashore"

b.
would match by

d[iou]g
would match: dig, dog, dug

d[^i]g
would match: dog and dug but not dig

d[a-c]g
will match patterns like dag, dbg, and dcg

d[A-C]g
will match dAg, dBg and dCg but not dag, dbg and dcg

4: read permission
2: write permission
1: execute permission
