while loop : will run till the condition is true
           
           cont=0
           num=10
           while [ $cont -le $num ]
           do 
              echo "Number is: $cont"
              let cont++
           done