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

-check the website connecctivity with ping command: 
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
            