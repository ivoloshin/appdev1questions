# App Developer 1 Questions

To answer these questions create an account at [repl.it](https://repl.it/). Select the language you are most comfortable with and create a session for each of the problems. Once your solutions are done, select share and send links to each of the solutions to the recruiter.

## Problem 1

Numbers in Mandarin follow 3 simple rules.
- There are words for each of the digits from 0 to 10.
- For numbers 11-19, the number is pronounced as "ten digit", so for example, 16 would be pronounced (using Mandarin) as "ten six".
- For numbers between 20 and 99, the number is pronounced as "digit ten digit", so for example, 37 would be pronounced (using Mandarin) as "three ten seven". If the digit is a zero, it is not included.

**Here is a mapping for the numbers between 0 and 10.**
```
'0': 'ling'
'1': 'yi'
'2': 'er'
'3': 'san'
'4': 'si'
'5': 'wu'
'6': 'liu'
'7': 'qi'
'8': 'ba'
'9': 'jiu'
'10':'shi'
```

Implement a function that converts an Arabic number (between 0 and 99), written as a string, into the equivalent Mandarin.

**Example Usage**
- `convert_to_mandarin('36')` will return `san shi liu`
- `convert_to_mandarin('20')` will return `er shi`
- `convert_to_mandarin('16')` will return `shi liu`

## Problem 2

We define super digit of an integer `x` using the following rules:

If `x` has only `1` digit, then its super digit is `x`.
Otherwise, the super digit of `x` is equal to the super digit of the digit-sum of `x`. Here, digit-sum of a number is defined as the sum of its digits.
For example, super digit of `9875` will be calculated as:

```
super_digit(9875) = super_digit(9+8+7+5) 
                  = super_digit(29) 
                  = super_digit(2+9)
                  = super_digit(11)
                  = super_digit(1+1)
                  = super_digit(2)
                  = 2.
```

You are given two numbers `n` and `k`. Implement a function that calculates the super digit of `P`.

`P` is created when number `n` is concatenated `k` times. That is, if `n=123` and `k=3`, then `P=123123123`.

**Input Format**

The function will take one **string** parameter containing two space separated integers, `n` and `k`. `n` should support numbers up to 32 digits. `k` should support numbers up to 

**Output Format**

Output the super digit of `P`, where `P` is created as described above.

**Example Usage**

`super_digit_sum('148 3')` will return `3`
`super_digit_sum('148 5')` will return `2`
`super_digit_sum('48652 2')` will return `5`

## Problem 3

You are given the following definitions:

- A run of monotonically increasing numbers means that a number at position `k+1` in the sequence is greater than or equal to the number at position `k` in the sequence.
- A run of monotonically decreasing numbers means that a number at position `k+1` in the sequence is less than or equal to the number at position `k` in the sequence.

Implement a function that takes a list of integers `L` containing at least `2` elements. The function finds the longest run of numbers in `L`, where the longest run can either be monotonically increasing or monotonically decreasing. In case of a tie for the longest run, choose the longest run that occurs first. The function does not modify the list. Function returns the sum of the longest run.

**Example Usage**

If `L = [10, 4, 3, 8, 3, 4, 5, 7, 7, 2]` then the longest run of monotonically increasing numbers in `L` is `[3, 4, 5, 7, 7]` and the longest run of monotonically decreasing numbers in `L` is `[10, 4, 3]`. Your function should return the value `26` because the longest run of monotonically increasing integers is longer than the longest run of monotonically decreasing numbers.

If `L = [5, 4, 10]` then the longest run of monotonically increasing numbers in `L` is `[4, 10]` and the longest run of monotonically decreasing numbers in `L` is `[5, 4]`. Your function should return the value 9 because the longest run of monotonically decreasing integers occurs before the longest run of monotonically increasing numbers.
