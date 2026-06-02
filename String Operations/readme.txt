String Operations 
to get a length of a string : s="hi my name is james"
                              len=${#s}
                              echo "length is $len"

to upper case the string    : upr=${s^^}
to lower case the string    : lwr=${s,,}
to repalce a word           : repl=${s/james/elon}
to get a value with index : sl=${s:3:4}    here 3 is starting and 4 is how much needed after starting number