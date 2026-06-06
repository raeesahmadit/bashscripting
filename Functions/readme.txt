Functions:
          block of code which perform some task and run when it is called
          reuseable also lessen our lines of code

          1:       function header {
                             echo "Welcome! to dream world"
                             }
    
          2:       footer() {
                        echo "Good Bye"
                            }

- to call a function just write the name of function

- function make and call with argument:
                    function header {
                             echo "Welcome! $1 to dream world"     #at $1 the given argument will be use
                             }
                
                   s= $(whoami)                          # $(whoami) will run as it is the linux command, store in s
                   header $s                             # $s value is argument to function
