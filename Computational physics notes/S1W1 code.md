# Reversing words

```
s =  "Hello world"

words = s.split()
print(words)

S = ""
for w in words:
  S += w[::-1] + " "

print(S)
```

#Remove elements from a list
We can use
- Pop()
- Remove()
- del()
```
L = [0,2,3,1,5]

#For loop
for i in L:
  print(i)
  L.pop(0)
  

print("-----------")

#While loop
index = 0
while index < len(L):
  print(L[index])
  index += 1
```

#POP

```
L = [0,2,3,1,5]

#For loop
counter = 0
for i in range(len(L)):
  print(L)
  L.pop()
```
