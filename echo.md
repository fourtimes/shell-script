```bash
echo "ashli joe"

output:
    ashli joe
```

```bash
without space:
--------------
echo -e "ashli \bjoe"

output:
    ashlijoe
```

```bash
one by one:
-----------
 echo -e "ashli \njoe"

output:
    ashli
    joe
```
```bash
with space:
-----------
echo -e "ashli \tjoe"

output:
    ashli 	joe
```

```bash
echo -e "Geeks \vfor \vGeeks"

output:- 
--------
Geeks 
      for 
          Geeks

```