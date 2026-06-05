while loop : will run till the condition is true
           
           cont=0
           num=10
           while [ $cont -le $num ]
           do 
              echo "Number is: $cont"
              let cont++
           done

Infinite loop: mostly use fo continous monitoring always the condition will true
              
             while true
             do 
                echo "Hi"
                sleep 2s
             done

Read a file using while loop:

             while read a
             do 
                echo "value is: $a"
             done < /home/ibtu/Desktop/name.txt                 #path of the file to read, only name the file if on the same location