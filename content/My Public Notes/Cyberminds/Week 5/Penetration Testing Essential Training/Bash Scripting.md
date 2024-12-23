# Basics in Bash
#### Print a variable on screen
```hello.sh
#!/bin/bash

str="Hello World"
echo $str
```
$>chmod +x hello.sh
$> ./hello.sh
Hello World

#### Print arguments form command line
```argue.sh
#!/bin/bash

echo $# //prints number of arguments
echo $1 $2 //prints the arguments itself
```
$>chmod +x argue.sh
$> ./argue.sh Hello World
2
Hello World

#### Variables in bash
```variables.sh
#!/bin/bash

num1=$1
num2=17
if [ $num1 -ge $num2]
then
	echo "Your value is greater than or equal to mine ($num2)"
else
	echo "My value ($num2) is greater than yours!"
fi
num3=$(($num1+$num2))
echo "Together they sum to $num3"
```
$>chmod +x variables.sh
$> ./variables.sh 19
Your value is greater than or equal to mine (17)
Together they sum to 36

#### Read in bash
```read.sh
#!/bin/bash

echo "What is your name? "
read name //different line
echo "Hello $name"
read -p "Remind me, what is your name? " name //same line
echo "Hello again $name"
```
$>chmod +x reader.sh
$> ./reader.sh
What is your name?
\>Malcolm
Hello Malcolm
Remind me, what is your name? \> Malcolm
Hello again Malcolm

---
# Controlling the flow in a script

```fortest.sh
#!/bin/bash

names=('Peter' 'Paul' 'Mary' 'David' 'Joe')
x=${#names[@]}
for (( i=0; i<$x; i++ ))
do
	echo ${names[${i}]}
done
```
$> ./fortest.sh
Peter
Paul
Mary
David
Joe

```wutest.sh
#!/bin/bash

runs=6
while [ $runs -gt 0 ]
do
	echo "Running down (while), now at $runs"
	let runs=runs-1
done

runs=1
until [ $runs -gt 6 ]
do
	echo "Running up (until), now at $runs"
	let runs=runs+1
done
```
$> ./wutest.sh
Running down (while), now at 6
Running down (while), now at 5
Running down (while), now at 4
Running down (while), now at 3
Running down (while), now at 2
Running down (while), now at 1
Running up (until), now at 1
Running up (until), now at 2
Running up (until), now at 3
Running up (until), now at 4
Running up (until), now at 5
Running up (until), now at 6

```iftest.sh
#!/bin/bash

if [ -d $1 ]
then
	echo $1 "exists"
	ls $1 -al
else
	echo $1 "doesn't exist"
fi
```
$> ./iftest.sh barney
barney doesn't exist
$> ./iftest.sh /usr/share/Thunar
/usr/share/Thunar exists
total 20
drwxr-xr-x   3  root  root  4096  AUg 21  2023 sendto

---
# Functions in bash

Single operator ('=') for string comparisons and assignments
Double operator ('\==') for numeric comparisons

```
#!/bin/bash

# Function that prints the language spoken in the city
function speak
{  if [$1 = "New York"]
   then
            echo "In New York, the primary language spoken is English."
   elif [$1 = "Tokyo"]
   then
            echo "In Tokyo, the primary language spoken is Japanese."
   else
		   echo "IDK"
   fi
}

# Display a menu of cities
PS3=">"
echo "Please select a city:"
select city in "New York" "Tokyo" "Paris" "Madrid" "Berlin" "Moscow" "Buenos Aires"
do
    if [ $city = "exit" ]
    then
	    echo "Invalid option. Please select a valid number."
        break
    fi
    case $city in
      New York)
        echo "Going to New York";;
    esac
    # Call the 'speak' function with the selected city name
	speak "$city"
done
```