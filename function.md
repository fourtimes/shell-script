```bash
normal function:
----------------
#!/bin/sh
test () {
   echo "Hello World"
}

test 

output:
    Hello World 

```

```bash
function with passing arguments:
--------------------------------
#!/bin/sh
one (){
   echo "Hi $1"
   echo "Hi $2"
}
one "ashli" "jino"

output:
   Hi ashli
   Hi jino

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

```bash
Global variable:
----------------
var="hello"
function foo(){
    echo $var
}
foo

   (or)

function foo()  {
    var="hello"
}
foo
echo $var

output:
   hello
```

```bash
Local variables:
----------------
function foo() {
    local var
    var="hello ash"
}
foo
echo $var

# output:
   hello ash
```