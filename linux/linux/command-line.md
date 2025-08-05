# Everything in linux is a file!
# Location of directories is called paths.
# `cd -` takes you back to the previoius direcoty you were just at.
# the `file` command tells you what type of file it is.
# the `cat` command is sho  rt for concatenate, it prints the contents of a file to the terminal.
# typing "h" inside a `less` command will show you the help menu.
# the `history` command shows you the history of commands you have typed.
# `!!` repeats the last command you typed. 
# `ctrl + r` allows you to search through your command history, keep pressing `ctrl + r` to go back through the history.
# `*` is a wildcard that matches any number of characters.
# `?` is a wildcard that matches a single character.
# `[]` is a wildcard that matches any single character in the brackets.
# using the `-i` flag will make some commands like `rm`, `mv` and `cp` interactive, meaning it will ask you for confirmation before executing the command incase a file is being overwritten or deleted.
# using the `-b` flag will make some commands like `mv` and `cp` create a backup of the file before overwriting it, the backup will have a `~` at the end of the filename.
# the `find` command accepts a `-name` flag and a `-type` flag, and it takes the search space as the first argument. i.e `find /home -type d -name someFolder` will search for directories named `someFolder` in the `/home` directory and its subdirectories recursively.
# you can use both the `help` command followed by the command name or the `man` command followed by the command name to get help on a specific command or the `--help` flag with the command to get help on a specific command, you can also use `man -k <keyword>` to search for commands related to a keyword.
# the `whatis` command gives you a one-line description of a command.
# use `alias` and `unalias` to create and remove aliases for commands, respectively.
# you can use `exit` or `logout` to exit the terminal session.



