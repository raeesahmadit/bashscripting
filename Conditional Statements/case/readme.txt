case:    it is like switch in other languages

          echo " choose an option :c=current location, d= date, f= files in current folder"
          
          read cho          
          case $cho in
             c)pwd;;
             d)  echo "today date is: "
                  date
                  echo "have a nice day";;
             f)ls;;
             *)echo "invalide entry"
          esac 