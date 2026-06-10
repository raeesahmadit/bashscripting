-basename : to get only file name from all given path used in bash
               basename /home/ibtu/Desktop/test.txt  # output        test.txt

-dirname : same as basename but use to get the directory name
               dirname /home/ibtu/Desktop/test.txt   #output        /home/ibtu/Desktop

-realpath : to get a path of a file
              realpath test.txt                      #output /home/ubtu/Desktop/text.txt

-check if file or directory is exist:

              if [ -d foldername]      if folder exist
              [ ! -d foldername]       if folder not exist

              if [ -f filename]        if file exist
              [ ! -f filename]         if file not exist

  example:   read -p "enter the file name: " a
             path="home/ibtu/Desktop/bashing/$a"
             if [[ -f $path ]]
             then 
                 echo "file exist"
             else
                 echo " file not exist!! do you want to make?"
                 read -p "press 0 to make and 1 to exit"
                 if [[ $q -eq 0 ]]
                 then 
                     touch $path
                     echo "$path: File is Created!!"
                 else 
                     echo "have a nice day"
                 exit
                 fi
              fi


-check the website connectivity with ping command: 
            read -p "enter website: " a
            ping -c 1 $a
            #sleep 2s
            if [[ $? -eq 0 ]]
            then 
               echo "$a connected successfully"
            else 
                 echo "unable to connect $a"
            fi

-check user is with UID:
             if [[ $UID -eq 0 ]]                #becasue root user id is 0
             then
             echo "Welcome Root!"
             else
             echo "you are not root user"
             fi

-random: also show random value between 0 to 32767
            echo $RANDOM
   example:
           n=$(( $RANDOM % 6 + 1 ))               #it will show number between 1-6 like dice
           echo "Number is: $n"

- to run a command on background even after close the terminal normaly files dtop when close the terminal

       nohup /filename.sh &