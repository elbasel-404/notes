# This appends text to a file
echo Hello World >> peanuts.txt 

# This overwrites the file
echo Hello World > peanuts.txt

# This redirects stdin instead of the terminal input to a file
cat < peanuts.txt > banana.tx

# this prints out an erro to the screen
ls /fake/directory > peanuts.txt 

# stdin = 1
# stdout = 2
# stderr = 3
