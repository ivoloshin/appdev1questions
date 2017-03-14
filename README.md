# App Developer Questions

To answer these questions create an account at [repl.it](https://repl.it/). Select a language you are most comfortable with and create a session for each of the problems. Once your solutions are done, select share and send links to each of the solution to the recruiter.

## Problem 1

Numbers in Mandarin follow 3 simple rules.
- There are words for each of the digits from 0 to 10.
- For numbers 11-19, the number is pronounced as "ten digit", so for example, 16 would be pronounced (using Mandarin) as "ten six".
- For numbers between 20 and 99, the number is pronounced as “digit ten digit”, so for example, 37 would be pronounced (using Mandarin) as "three ten seven". If the digit is a zero, it is not included.

Here is a mapping for the numbers between 0 and 10.
```
'0':'ling'
'1':'yi'
'2':'er'
'3':'san'
'4': 'si'
'5':'wu'
'6':'liu'
'7':'qi'
'8':'ba'
'9':'jiu'
'10': 'shi'
```

We want to write a procedure that converts an American number (between 0 and 99), written as a string, into the equivalent Mandarin.
________________________________________
Example Usage:
- `convert_to_mandarin('36')` will return `san shi liu`
- `convert_to_mandarin('20')` will return `er shi`
- `convert_to_mandarin('16')` will return `shi liu`

