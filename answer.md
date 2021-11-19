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

## Problem 4

Answer

```bash
#!/bin/bash

SEQ=SEQ_FILE
if [[ ! -s $SEQ ]]
then
        touch $SEQ
        echo 1 > $SEQ
fi
value=$(cat $SEQ)
echo $((value+1)) > $SEQ
echo $valu
```

## Problem 5

Answer

```bash
cat FILE_NAME | awk 'BEGIN{sum=0} {sum=sum+$1} END{print sum}'
```
