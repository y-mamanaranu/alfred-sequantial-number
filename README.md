# Alfred Sequential Number
An Alfred workflow to generate sequential numbers.

<img width="764" alt="screenshot" src="https://github.com/user-attachments/assets/f7865355-b661-4c4a-8024-df26e789ab8b" />


## Usage

- `%b`: binary
- `%o`: octal
- `%d, #`: decimal
- `%x`: hexadecimal in lower case
- `%X`: hexadecimal in upper case
- `%a, #a`: alphabetic in lower case: a, b, c, ...
- `%A, #A`: alphabetic in upper case: A, B, C, ...

### `seq`
```
seq <length or range>

seq 10
>>> 1 2 3 ... 8 9 10
seq 3-10
>>> 3 4 5 ... 8 9 10
```
Generate sequential numbers with specified length or range.
Same as `seq fmt %d`.

### `seq bin`
```
seq bin <length or range>

seq bin 10
>>> 1 10 11 ... 1000 1001 1010
seq 3-10
>>> 11 100 101 ... 1000 1001 1010
```
Generate sequential numbers in binary with a specified length or range.
Same as `seq fmt %b` and `seq fmt #`.

### `seq oct`
```
seq oct <length or range>

seq oct 8
>>> 1 2 3 ... 6 7 10
seq oct 3-8
>>> 3 4 5 ... 6 7 10
```
Generate sequential numbers in octal with a specified length or range.
Same as `seq fmt %o`.

### `seq hex`
```
seq hex <length or range>

seq hex 16
>>> 1 2 3 ... e f 10
seq hex 3-16
>>> 3 4 5 ... e f 10
```
Generate sequential numbers in hexadecimal in lower cases with a specified length or range.
Same as `seq fmt %x`.

### `seq Hex`
```
seq Hex <length or range>

seq Hex 8
>>> 1 2 3 ... E F 10
seq Hex 3-8
>>> 3 4 5 ... E F 10
```
Generate sequential numbers in hexadecimal in upper cases with a specified length or range.
Same as `seq fmt %X`.

### `seq alf`
```
seq alf <length or range>

seq alf 27
>>> A B C ... y z aa
seq alf 3-27
>>> C D E ... y z aa
```
Generate sequential numbers alphabetically in lower cases with a specified length or range.
Same as `seq fmt %a` and `seq fmt #a`.

### `seq Alf`
```
seq Alf <length or range>

seq Alf 27
>>> A B C ... Y Z AA
seq Alf 3-27
>>> C D E ... Y Z AA
```
Generate sequential numbers alphabetically in upper cases with a specified length or range.
Same as `seq fmt %a` and `seq fmt #a`.

### `seq fmt`
```
seq fmt <format> <length or range> [<length or range> ...]

seq fmt Sample-#a-# 3 2
>>> Sample-a-1 Sample-a-2 Sample-b-1 Sample-b-2 Sample-c-1 Sample-c-2
```
Generate sequential numbers alphabetically in upper cases with a specified length or range.
