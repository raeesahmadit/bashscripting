for loop : 
integer:
          for i in 1 2 3 4 5 6 7 8 9 10
          do 
             echo "Number is: $i"
          done
 or
          for i in {1..5}
          do 
            echo "Number is: $i"
          done

string:
          for name in raees ahamd qundeel iblu umaima
          do 
            echo "Name is: $name"
          done

getting values from file: 

                    file_path="/home/ibtu/Desktop/bashing/name.txt"
                    for nam in $(cat $file_path)
                    do 
                    echo "Name of employee: $name"
                    done

for loop in aarays:
                    myarray=(2 4 6 8 10 hello nvidia)
                    length=${#myarray[*]}
                    for ((i=0;i<$length;i++))
                    do
                        echo "Value of aaray is: ${myarray[$i]}"
                    done

infinite loop:
                 for (( ;; ))
                 do 
                     echo "hi raees"
                     sleep 2s                                 #it will pause for 2 sec
                  done