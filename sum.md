#Given a three-digit number. Find the sum of its digits.

```
Example input
123

Example output
6
```

num = int(input())

a = (num%10)

b = ((num//10)%10)

c = ((num//10)//10)

sum = a + b + c

print(sum)
