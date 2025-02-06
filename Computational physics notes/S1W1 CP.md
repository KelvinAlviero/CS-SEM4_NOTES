

# PHYTHON IS LAZY!!
Sir Zhandos 2025

# Short summary
We learnt about variable tupes, inputting data into a variable , Controlling programs, Binary operations, true and false, lists and arrays, range.

#Variable types
- Integer
- Float
- Complex (X = complex(1.5))

Math libary is used for various mathimatical fuctions(Log, pi)

# True and false
- False  =  {0, None, []}
- WTrue = {Anything that isn't false)

# Betowice comparions, compares binary things. 
```
1 1 0 1 0
1 0 0 1 0
---------
1 0 0 1 0
```

# break or continue
```
for i in range (n);
  if i % 2 ==  0;
    break
    print 2 x i
  else :
   continue
    print i
```
- (If even it goes to the break statement, if odd it prints "i")

Infinite loop
-Uses "While true"
(Refer to "True and False)

##LISTS
-Ordered collection of variables and numbers, it is FLEXIBLE
A = [ 0, 1 ,hi ,[]]

##ARRAYS
- a FIXED size of a list
```
L1 = [1,2,3,4,5]
L2 = L1
L2[0] = -1
print (L1)
print (L2)

[-1,2,3,4,5]
[-1,2,3,4,5]
```
-------------------
```
L1 = [1,2,3,4,5]
L2 = list(L1)
L2[0] = -1
print (L1)
print (L2)
  
[1,2,3,4,5]
[-1,2,3,4,5]
```
-------------------
```
L1 = [1,2,3,[0,0,0],5]
L2 = list(L1)
L2[0] = -1
L2 [3][0]= 1 
L2 [3][1]= 1 
L2 [3][2]= 1 
print (L1)
print (L2)
  
[1,2,3,[1,1,1],5]
[-1,2,3,[1,1,1],5]

```
We can see L1 and L2 are the same, in this case *deepcopy* is needed
```
L1 = [1,2,3,[0,0,0],5]
L2 = copy.deepcopy(list(L1))
L2[0] = -1
L2 [3][0]= 1 
L2 [3][1]= 1 
L2 [3][2]= 1 
print (L1)
print (L2)
  
[1,2,3,[0,0,0],5]
[-1,2,3,[1,1,1],5]
```
#For loops
```
for i in range (10):
  print(i)
(Prints from 0 - 10)
```
Here, range creates a sequence from 0 to 9

# User defined functions
```
def f(n):
  print(n)
  return (n+1):

f(10)
```
Return is needed to give back an answer, without "(n+1)" it gives nothing but still works, without return at all, the code still works, kinda.
```
def f(n):
  if n % 2 = 0 :
    return
  else
    print (n)
    return n + 1
  print('done')
```
f(10)= done
f(11) = None,11,12

For even numbers it gives a none...

