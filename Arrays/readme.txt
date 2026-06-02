Arrays : to store multiple values at once

make an array : myarray=(1 2 3 hello "Ahmad")

to retrive all values : echo "all values are ${myarray[*]}"

to get a length of array : echo ${#myarray[*]}

to retrive perticular values : echo "God is ${myarray[0]} and my legs are ${myarray[1]} triangle have ${myarray[2]} corners my name is ${myarray[4]}"

to retrive a range of values (2-4 only): echo "values from 2 to 4 is : ${myarray[*]:2:2}"
                                                                      first 2 is starting and second 2 is how much values after starting
                                                                      so we are asking 2 to 4 so start form 2 and then 2 values
to update an array : myarray+=(30 40)
                     echo "new updated array is ${myarray[*]} and new length is ${#myarray[*]}" 

key values pairs : to retrive value with name instead of index number
    make a array : declare -A myarrays
                   myarrays=([name]=raees [age]=30 [city]=fsd)
                   echo "name is ${myarrays[name]}"
                   echo "age is ${myarrays[age]}"