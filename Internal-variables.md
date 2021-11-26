```bash
$* (or) $@:
-----------
"$*" is the same as "$1 $2 ..." 1
"$@" is the same as "$1" "$2" ...

vim file - a.sh
    #!/usr/bin/env bash
    echo "$*"

run the file:-
    bash a.sh "joe jino ashli"

ouput:-
    # joe jino ashli

                    (or)

vim file - a.sh
    #!/usr/bin/env bash
    echo "$@"

run the file:-
    bash a.sh "joe" "jino" "ashli"

ouput:-
    # joe jino ashli
```

```bash
$#:-
----
Number of positional parameters passed to the script or function.

vim file - a.sh
    #!/usr/bin/env bash
    echo "$#"

run the file:-
    bash a.sh joe jino ashli kulandai joseph

ouput:-
    # 5
```

```bash
$HISTSIZE:
---------
The maximum number of remembered commands.

run the command in terminal:
     echo $HISTSIZE

# output:
    1000
```

```bash
$FUNCNAME:
----------

vim file - a.sh
    #!/usr/bin/env bash
    my_function()
    {
        echo "This function is $FUNCNAME"
    }
    my_function

run the file :
    bash a.sh

# output:
    This function is my_function
```

```bash
$IFS:
-----
Contains the Internal Field Separator string that bash uses to split strings when looping etc. The default is the white space characters: \n (newline), \t (tab) and space.

vim file - a.sh
    #!/usr/bin/env bash
    IFS=","
    INPUTSTR="a,b,c,d"
    for field in ${INPUTSTR}; do
        echo $field
    done

run the file:
    bash a.sh

# output:
    a
    b
    c
    d
```

```bash
$OLDPWD:
--------
OLDPWD (OLDPrintWorkingDirectory) contains directory before the last cd command.

    ~> $ cd directory
    directory> $ echo $OLDPWD

# output:
    /home/ubuntu
```

```bash
$1 $2 $3 etc..
--------------
Positional parameters passed to the script from either the command line or a function:

vim file - a.sh
    #!/bin/bash
    # $n is the n'th positional parameter
    echo "$1"
    echo "$2"
    echo "$3"

run the file:
    bash a.sh ashli joe nive

# output:
    ashli
    joe
    nive
```

```bash
$?:
---
The exit status of the last executed function or command. Usually 0 will mean OK anything else will indicate a
failure:

Ex:1
    ~> $ ls *.blah;echo $?
    # ls: cannot access *.blah: No such file or directory
    # 2

Ex:2
    ~> $ ls;echo $?
    # a.sh  ashli  file.txt  one.txt  test.sh  two.txt  v.sh  var.sh
    # 0

```

```bash
$$:
---
The Process ID (pid) of the current process.

run the command in terminal:
    echo $$

# output:
    13246
```

```bash
$RANDOM:
--------
Each time this parameter is referenced, a random integer between 0 and 32767 is generated. Assigning a value to this variable seeds the random number generator (source).

run the command in terminal:
    echo $RANDOM
    # 27119

    echo $RANDOM
    # 1349
```

```bash
$BASHPID:
---------
Process ID (pid) of the current instance of Bash. This is not the same as the $$ variable, but it often gives the same
result.

run the command in terminal:
    echo "\$\$ pid = $$  BASHPID = $BASHPID"
    # $$ pid = 9265  BASHPID = 9265
```

```bash
$BASH_VERSINFO:
---------------
n array containing the full version information split into elements, much more convenient than $BASH_VERSION if
you are just looking for the major version.

run the command in terminal:
     for ((i=0; i<=5; i++)); do echo "BASH_VERSINFO[$i] = ${BASH_VERSINFO[$i]}"; done

# output:
BASH_VERSINFO[0] = 3
BASH_VERSINFO[1] = 2
BASH_VERSINFO[2] = 25
BASH_VERSINFO[3] = 1
BASH_VERSINFO[4] = release
BASH_VERSINFO[5] = x86_64-redhat-linux-gnu
```

```bash
$SECONDS:
---------
The number of seconds a script has been running. This can get quite large if shown in the shell:

run the command in terminal:
    echo $SECONDS

# output:
    98834
```

```bash
$UID:
-----
A read only variable that stores the users ID number.

run the command in terminal:
     echo $UID

# output:
    12345
```
