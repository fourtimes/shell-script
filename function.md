```bash

#!/bin/sh
test () {
   echo "Hello World"
}

test 

output:
    Hello World 

```

```bash
Nested Function:
----------------
#!/bin/sh
number_one () {
   echo "This is the first function speaking..."
   number_two
}

number_two () {
   echo "This is now the second function speaking..."
}

number_one

output:
    This is the first function speaking...
    This is now the second function speaking...
```