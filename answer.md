## Problem 1

Answer

```bash
md5sum
```

## Problem 2

Answer

```bash
diff file1 file2
```

## Problem 3

Answer

```bash
#!/bin/bash

input=${1:-please enter a number}
expr $input + 0 &>/dev/null
if [[ $? -ne 0 ]]
then
        echo $input
elif [[ $((input % 2)) -eq 0 ]]
then
        echo "even"
else
        echo "odd"
fi
```
