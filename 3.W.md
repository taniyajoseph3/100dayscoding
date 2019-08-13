# Write a program that receives a number on the input and prints values from 1 to   
that number subjected to the conditions below. 
```
INPUT 
5
0
OUTPUT
1
2
Jugs
4
Mugs

INPUT 
15
1
OUTPUT
1
2
Jugs
4
Mugs
Jugs
Pugs
8
Jugs
Mugs
11
Jugs
Jugs
Pugs
MugsJugs
```
num = int(input())
rev = int(input())
for i in range(1,num+1):
  if rev: 
    string = 'Jugs' * bool(i%3==0 or '3' in str(i))
    string = 'Mugs' * bool(i%5==0 or '5' in str(i)) + string 
    string = 'Pugs' * bool(i%7==0 or '7' in str(i)) + string 
    print( string or i)
  else: 
    print("Jugs" * (i%3==0 or '3' in str(i)) + "Mugs" * (i%5==0 or '5' in str(i)) + "Pugs" * (i%7==0 or '7' in str(i)) or i)
