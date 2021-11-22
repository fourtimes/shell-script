```bash
1. file name - var.sh
    #!/bin/sh
    MY_MESSAGE="Hello World"
    echo $MY_MESSAGE

2. run the file - bash var.sh
# output: hello world
```

```bash
**Unsetting Variables:-----**

1. file name - test.sh
    #!/bin/sh
    NAME="Zara Ali"
    unset NAME
    echo $NAME

2. run the shell script file - bash test.sh
# output: (empty values)
```
