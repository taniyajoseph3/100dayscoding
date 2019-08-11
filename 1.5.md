#N students take K apples and distribute them among each other evenly. The remaining (the indivisible) part remains in the basket. How many apples will each single student get? How many apples will remain in the basket?


```
Example input
6
50

Example output
8
2
```
a = int(input()) 
b = int(input()) 
print(b // a) 
print(b % a)
