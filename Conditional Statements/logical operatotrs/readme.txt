&& : 
    read -p "Enter age:" age
    read -p "Enter country: " count
    if [[ $age -ge 12 ]] && [[ $count == "america" ]]                     # == use for string,    -eq for numeric
      then
       echo "You can vote"
    else
      echo "come back next year only if you are american"
    fi

|| : 
    read -p "Enter age:" age
    read -p "Enter country: " count
    if [[ $age -ge 25 ]] || [[ $count == "america" ]]
      then
      echo "You can vote"
    else
      echo "come back next year buddy!!"
    fi  