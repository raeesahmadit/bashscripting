>    >> : to direct a output in a file 

        ls > filename.txt   #overwrite
        date > date.txt
        pwd >> date.txt     #write after previous data


/dev/null : if you dont want to print output of a command on terminal or write in a filename
        
        - cd /root/                        #permision denied
        - cd /root/ &> /dev/null           #it will show nothing


-print name of a script you are using:
                  echo "you are using ${0} script"

-log message : if you want to maintain the logging for script, you can use logger
             logger "this is log from ${0}"                       #logger is keyword  
                    then go to: sudo less /var/log/messages       #to see the log of your file in it

debugging script: to enable debugging in script, when make big files you can see step by step commands
            set -x :        at the starting of a file to enable debugging
            set -e :        stop the file at the point where error occur