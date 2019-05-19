# Get familiar with some command line utils

## Advise

Please document your solutions

## Preparation

Create your folder work the exercises:

```sh
mkdir ~/exercises
```

## Grep

### Grep lines from a file containing a specific substring (case sensitive)

```sh
cd
mkdir ~/exercises/grep-1 && cd ~/exercises/grep-1
echo $'A\nB1\nB2\nb\nC' > file.txt
```

Input file `file.txt`

```txt
A
B1
B2
b
C
```

Grep all lines that contain a `B`

`grep <YOUR_PART_OF_THE_SOLUTION> file.txt`

Expectd Result
```txt
B1
B2
```

### Grep lines from a file containing a specific substring (case insensitive)

Grep all lines that contain a `B` or `b`

`grep <YOUR_PART_OF_THE_SOLUTION> file.txt`

Expectd Result
```txt
B1
B2
b
```


### Grep lines from a file not containing a specific substring

```sh
mkdir ~/exercises/grep-2 && cd ~/exercises/grep-2
echo $'A\nB1\nB2\nC' > file.txt
```

Grep all lines that do not contain `B`

`grep <YOUR_PART_OF_THE_SOLUTION> file.txt`

Expectd Result

```txt
A
b
C
```

### Grep all lines that start with a number

```sh
mkdir ~/exercises/grep-2 && cd ~/exercises/grep-2
echo $'1\nA1\n2\n3\nB1' > file.txt
```

Input file `file.txt`

```txt
1
A1
2
3
B1
```

`grep <YOUR_PART_OF_THE_SOLUTION> file.txt`

Expectd Result

```txt
1
2
3
```

### Count the lines that start with a number

`grep <YOUR_PART_OF_THE_SOLUTION> file.txt`

Expectd Result

```txt
3
```


### Grep only matching part of string

Input `I had two beers for $12 and a steak for $35`

```sh
echo 'I spent $120 on the weekend' | grep <YOUR_PART_OF_THE_SOLUTION>
```

Expected output

```
$120
```

## Sed

## Replace name in string with another name

Replace `Hans` with `Dieter` in `I had a meeting with Hans`

```sh
echo 'I had a meeting with Hans' | sed <YOUR_PART_OF_THE_SOLUTION>
```

Expected output

```txt
I had a meeting with Dieter
```

## Replace each number in string

Replace each digit `0-9` with a `#` in `I had two beers for $12 and a steak for $35`

```sh
echo 'I had two beers for $12 and a steak for $35' | sed <YOUR_PART_OF_THE_SOLUTION>
```

Expected output

```txt
I had two beers for $## and a steak for $##
```

## tr

### Delete a character from string

Input

```txt
Apple, Banana, Coconut
```

Delete the comma from the input.

```sh
echo 'Apple, Banana, Coconut' | tr <YOUR_PART_OF_THE_SOLUTION>
```

expected result

```txt
Apple Banana Coconut
```

### Replace a character with another

Input 

```txt
Apple, Banana, Coconut
```

Replace the comma from the input with a semicolon.

```sh
echo 'Apple, Banana, Coconut' | tr <YOUR_PART_OF_THE_SOLUTION>
```

expected result

```txt
Apple; Banana; Coconut
```
