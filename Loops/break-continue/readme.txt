break: to stop a loop

    read -p "enter finding number:" n
    for i in {1..10}
    do
         if [[ $n -eq $i ]]
          then
          echo "$n is found!!"
          break
          fi
          echo "the number is $i"
    done




continue:  to stop current iteration of loop and start next iteration
         read -p "enter range start: " a
         raed -p "enter range end: " b
         for ((i=$a;i<$b;i++))
         do
           let o=$i%2
           if [[ $o -eq 0 ]]
           then 
           continue
           fi
           echo "Odd no. $i"
         done

