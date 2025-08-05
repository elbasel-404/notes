# `stdin` is standart input ( by default it is the keyboard ), `stdout` is standard output (    by default it is the screen ), and `stderr` is  standard error ( by default it is the screen ).
# you can use the `>` operator to redirect the output of a command to a file. i.e `echo "Hello, World!" > output.txt`, this will overwrite the file `output.txt` with the text "Hello, World!". If you want to append to the file instead of overwriting it, you can use the `>>` operator, i.e `echo "Hello, World!" >> output.txt`. or use the flag 
# the `<` operator is used to redirect the input of a command from a file. i.e `cat < input.txt`, this will read the contents of the file `input.txt` and print it to the screen, you can combine the two operators to read from a file and write to a file, i.e `cat < input.txt > output.txt`, this will read the contents of the file `input.txt` and write it to the file `output.txt`.
# the file descriptor `0` is used for standard input, `1` is used for standard output, and `2` is used for standard errorr.
# to redirect stderr to a file you can use `ls /fake/dir 2> peanuts.txt` 
# you can redirect streams to another stream using `streamToRedirect>&1`. i.e to redirect stderr to stdout you can use 2>&1.
# $ ls /fake/directory > peanuts.txt 2>&1
# his sends the results of ls /fake/directory to the peanuts.txt file and then it redirects stderr to the stdout via 2>&1. The order of operations here matters, 2>&1 sends stderr to whatever stdout is pointing to. In this case stdout is pointing to a file, so 2>&1 also sends stderr to a file. So if you open up that peanuts.txt file you should see both stderr and stdout. In our case, the above command only outputs stderr.
# a shorted way to redirect both stdout and stderr to a file is `ls /some/fake/dir &> peanuts.txt`
# `ls /some/fake/dir 2> /dev/null`
# ls /some/fake/dir > output.txt 2> error.txt
# `ls -la /etc/ | less` pipes the stdout of a command to the stdin of another command
# `ls | tee peanut.txt` will outpuot ls to the screen and the file.
# View all your enviroment variable by using `env`
# PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/bin is a list of paths seperated by a colon that the system looks into for binaries to run when you run a command from the terminal.
$ echo 'The quick brown; fox jumps over the lazy  dog' > sample.txt
# cut -c 5 "hello" outputs "o" which is the firth char but hello must be file
# cut can be used by fields. `cut -f 1 -d " " sample.txt", let's say sample.text contains "hello yay noo"
since it splits text by the delimiter ( space ) and we are selecting the 1st field, the output wll be "hello"
# paste takes a multilne file and turns into a one-line string.
if you have a file: 
```
first line
second line
third line
```
and then you ran `paste -d ' ' -s fileName` you will get `first line  second line third line`

---

`head` will show you the first n lines inside a file, useful for long files
head -n 15 /var/log/...

---

`tail` will show you the last n lines inside a file.
`tail -n 15 /var/log...`
you can also use `-f` to "follow" the file changes

---

use `expand` to turn all tabs inside a file to spaces instaheadead.
`expand fileName > outputFileName`
use "unexpand" does the opposite
`unexpand -a result.txt`

---





