```bash
if Statement:
-------------
a=10
b=20
  
if [ $a == $b ]
then
    echo "a is equal to b"
fi
  
if [ $a != $b ]
then
    echo "a is not equal to b"
fi

output: 
    a is not equal to b

```

```bash
if else statement:
------------------
#Initializing two variables
a=20
b=20
  
if [ $a == $b ]
then
    #If they are equal then print this
    echo "a is equal to b"
else
    #else print this
    echo "a is not equal to b"
fi

output:
    a is equal to b
```

```bash
if else statement using AND condition:
-------------------------------------

#!/bin/bash
 
read -p "Enter First Numeric Value: "  first
read -p "Enter Second Numeric Value: "  second
 
if [ $first -le 10 ]  && [ $second -gt 20 ]
then
    echo "Both conditions are true"
else
    echo "Atleast one conditions is false"
fi

output:
Enter the first numeric value: 6
Enter the second numeric value: 38
    **Both conditions are true**
```


```bash
if else statement using OR condition:
-------------------------------------
#!/bin/bash

read -p "Enter First Numeric Value: " first
read -p "Enter Second Numeric Value: " second

if [ $first -le 10 ] || [ $second -gt 20 ]
then
    echo "Atleast one conditions is true"
else
    echo "Both conditions are failed"
fi

output:
Enter the first numeric value: 6
Enter the second numeric value: 38
    **Atleast one conditions is true**
```