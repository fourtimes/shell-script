```bash
CARS="bmw"

#Pass the variable in string
case "$CARS" in
    # case 1
    "creta") echo "This is creta car company" ;;

    # case 2
    "audi") echo "This is audi car company" ;;

    #c ase 3
    "bmw") echo "This is bmw car company" ;;
esac

output:
    => This is bmw car company
```
