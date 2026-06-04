if else : 

        if [[ $marks -gt 40 ]]          # space should be between [[ value ]]
        then 
            echo "You are pass"
        else 
            echo "you are fail"
        fi                               # this is to end the condition

       " -gt      = greter than
         -lt      = less then
         !=       = not equal
         -le      = less then and equal to
         -ge      = greater than and equal to
         ==/-eq   = equal to
       "

elif : if [[ $age == 0 ]]
       then 
         echo "you are not born yet!"
       elif [[ $age -ge 50 ]]
       then
         echo "you are living a bonus life"
       elif [[ $age -lt 12 ]]
       then 
         echo "you are just a kid :)"
       else
         echo "you are young"
        fi