```bash
while conditions:
-----------------
Example:- 1

    #!/bin/sh
    a=0
    while [ $a -lt 10 ]
    do
        echo $a
        a=`expr $a + 1`
    done

# output:-
    0
    1
    2
    3
    4
    5
    6
    7
    8
    9

Example:- 2
    #!/bin/sh
    a=10
    while [ $a -ge 0 ]
    do
       echo "Reverse order number $a"
       let a--;
    done

output:
    Reverse order number 10
    Reverse order number 9
    Reverse order number 8
    Reverse order number 7
    Reverse order number 6
    Reverse order number 5
    Reverse order number 4
    Reverse order number 3
    Reverse order number 2
    Reverse order number 1
    Reverse order number 0

```
