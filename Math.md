```bash
echo '3 3 + p' | dc
    (or)
dc <<< '3 3 + p'

output:
    6
```
```bash
dc <<< '1 1 + p 2 + p'

output:
    2
    4
```
```bash
dc <<< '4 3 / p'

output:
    1
```

```bash
Multiplication:
---------------
echo $((5 * 2))

output:
10
```

```bash
Division:
---------
echo $((5 / 2))

output:
    2
```

```bash
Modulo:
-------
echo $((5 % 2))

output:
    1
```

```bash
Exponentiation:
---------------
echo $((5 ** 2))

output:
    25
```

