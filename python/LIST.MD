**1. Write a program to enter 10 numbers in a list and print sum of all even and odd numbers.**
```
L = []
for i in range(10):
    num = int(input('Enter a number: '))
    L.append(num)

even_sum, odd_sum = 0, 0
for i in L:
    if i % 2 == 0:
        even_sum += i
    else:
        odd_sum += i

print('Sum of all even numbers =', even_sum)
print('Sum of all odd numbers =', odd_sum)
```

**2. Write a program to enter 10 numbers in a list and print the greatest and smallest number.**
```
L = []
for i in range(10):
    num = int(input('Enter a number: '))
    L.append(num)

g, s = L[0], L[0]
for i in L:
    if i > g:
        g = i
    elif i < s:
        s = i

print('Greatest number =', g)
print('Smallest number =', s)
```

**3. Write a program to enter 10 numbers in a list and print all consecutive numbers.**
```
L = []
for i in range(10):
    num = int(input('Enter a number: '))
    L.append(num)

for i in range(9):
    if L[i] + 1 == L[i+1]:
        print(L[i], L[i+1])
```

**4. Write a program to enter 10 numbers in a list and print all prime numbers.**
```
L = []
for i in range(10):
    num = int(input('Enter a number: '))
    L.append(num)

for i in L:
    prime = True
    for j in range(2, i):
        if i % j == 0:
            prime = False
            break

    if prime == True:
        print(i, end=' ')
```

**5. Write a program to enter 10 numbers in a list and print sum of all numbers ending with 0.**
```
L = []
for i in range(10):
    num = int(input('Enter a number: '))
    L.append(num)

sum = 0
for i in L:
    if i % 10 == 0:
        sum += i

print(sum)
```

**6. Write a program to enter 10 numbers in a list, then ask the user to search a number. If number is available print found else print not found.**
```
L = []
for i in range(10):
    num = int(input('Enter a number: '))
    L.append(num)

val = int(input('Enter a number to search: '))
found = False

for i in L:
    if val == i:
        print('Found')
        found = True
        break

if found == False:
    print('Not Found')
```

**7. Write a program to enter 10 numbers in a list and reverse the list.**
```
L = []
for i in range(10):
    num = int(input('Enter a number: '))
    L.append(num)

f = 0
r = len(L) - 1

while f < r:
    temp = L[f]
    L[f] = L[r]
    L[r] = temp
    f += 1
    r -= 1

print(L)
```

**8. Write a program to enter 10 numbers in a list and print frequency of each number.**
```
L = []
for i in range(10):
    num = int(input('Enter a number: '))
    L.append(num)
```

**9. Write a program to enter 10 numbers in a list and arrange the list so that first number will shift at last and rest number will shift 1 index before.**
```
L = []
for i in range(10):
    num = int(input('Enter a number: '))
    L.append(num)

for i in range(9):
    temp = L[i]
    L[i] = L[i+1]
    L[i+1] = temp

print(L)
```

**10. Write a program to enter 10 numbers in a list and print the list in ascending order.**
```
L = []
for i in range(10):
    num = int(input('Enter a number: '))
    L.append(num)

g, s = L[0], L[0]
for i in L:
    if i > g:
        g = i
    elif i < s:
        s = i

for i in range(s, g+1):
    for j in L:
        if i == j:
            print(i, end=' ')
```

**11. Write a program to enter 10 numbers in a list and print the list in descending order.**
```
L = []
for i in range(10):
    num = int(input('Enter a number: '))
    L.append(num)

g, s = L[0], L[0]
for i in L:
    if i > g:
        g = i
    elif i < s:
        s = i

for i in range(g, s-1, -1):
    for j in L:
        if i == j:
            print(i, end=' ')
```

**12. Write a program to enter 10 numbers in a list and print whether it is in ascending, descending or no order.**
```
L = []
for i in range(10):
    num = int(input('Enter a number: '))
    L.append(num)

asc = True
for i in range(9):
    if L[i] > L[i+1]:
        asc = False
        break

desc = True
for i in range(9):
    if L[i] < L[i+1]:
        desc = False
        break

if asc == True:
    print('Ascending order.')
elif desc == True:
    print('Descending order.')
else:
    print('No order.')
```
