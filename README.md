# python
# swap
a=1
b=2
a,b=b,a
print(a,b)

# swap temp
a=1
b=2
temp=a
a=b
b=temp
print("a:",a)
print("b:",b)

# swap op using +,-,*,/
a=int(input("enter the value of a:"))
b=int(input("enter the value of b:"))
a=a+b
b=a-b
a=a-b
print(a)
print(b)

# range
for i in range(51):
  print("i",end=" ")

word=input("enter a word:")
for ab in word:
  print(ab)

for i in range(10,-1,-1):
  print(i,end=" ")

# swap *,/
a=int(input())
b=int(input())
a=a*b
b=a/b
a=a/b
print()
print(a)
print(b)

# list
fruits=['apple','mango','cherry']
print(fruits)
print(fruits[1])
fruits[2]='kiwi'
print(fruits)

# list index
nums=[0,1,2,3,4,5]
print(len(nums))
print(nums[1:5])
print(nums[:3])
print(nums[::2])
print(nums[::-1])

#  sort reverse
fruits=['apple','mango','cherry']
fruits.sort()
print(fruits)
fruits.reverse()
print(fruits)

# index
nextnum=[[1,2],[3,4],[5,6]]
print(nextnum[1])
print(nextnum[2][0])

# reverse str
text='india won'
words=text.split()
w1=words[0][::-1]
w2=words[1][::-1]
result=''.join([w1,w2])
print(result)

# nested dict
loc={
    (40.1234,-75.00001):"NewYork",
    (34.1223,-111.345):"vijaywada"
}
print(loc[(34.1223,-111.345)])

# set impementations
set_1={1,2,3,4,5}
print(set_1)
print("add and remove elements")
set_1.add(6)
print(set_1)
set_1.remove(2)
print(set_1)
print(3 in set_1)
print(10 not in set_1)
#
a={1,2,3}
b={3,4,5}
print("union:",a.union(b))
print("intersection:",a.intersection(b))
print("difference:",a.difference(b))
print("symmetricdiff:",a.symmetric_difference(b))

subset check
a={1,2}
b={1,2,3,4,5}
print("a is subset to b:",a.issubset(b))
print("b is subset to b:",b.issubset(a))

# by using conditional op
a={1,2}
b={1,2,3,4,5}
print("subset or not:",a<=b)
print("proper subset:",a<b)
print("superset or not:",a>=b)
print("proper superset:",b>a)

# set with lists
nums=[1,2,2,5]
single=set(nums)
print(single)
#
x=set([1,2])
y=set([1,2,3])
if x.issubset(y):
    print("x is a subset od y")

   # 
  info={'name':'india','num':123}
s=123
for key,value in info.items():
    if value==s:
        print(f"key for value:'(s)':{key}")


# armstrong number

a=int(input("enter the number"))
temp=a
n=len(str(a))
sum=0
while temp>0:
  digit=temp%10
  sum+=digit**n
  temp//=10
print("latest value of sum:",sum)
print("latest value of temp:",temp)
if sum==a:
  print("armstrong number")
else:
  print("not an armstrong number")

# niven's / harshad

a=int(input("enter the number"))
temp=a
sum=0
while temp>0:
  digit=temp%10
  sum+=digit
  temp//=10
  print("latest value of sum:",sum)
  print("latest value of temp:",temp)
if a%sum==0:
  print("harshad number")
else:
  print("not a harshad number")

for i in "teju":
  print(i)

# patterns 

n=int(input("enter the size"))
for i in range(n):
  for j in range(n):
    print("*",end=" ")
  print()
  
###
n=int(input("enter the size"))
for i in range(n):
  for j in range(n):
    if i==0 or i==n-1 or j==0 or j==n-1:
      print("*",end=" ")
    else:
      print(" ",end=" ")
  print()

# for anti diagonal
n=int(input("enter the size"))
for i in range(n):
  for j in range(n):
    if i==0 or i==n-1 or j==0 or j==n-1 or i==j or i+j==n-1:
      print("*",end=" ")
    else:
      print(" ",end=" ")
  print()

# for diagonal

  n=int(input("enter the size"))
for i in range(n):
  for j in range(n):
    if i==0 or i==n-1 or j==0 or j==n-1 or i==j:
      print("*",end=" ")
    else:
      print(" ",end=" ")
  print()

 # butterfly
 
 n=int(input("enter the size"))
for i in range(n):
  for j in range(n):
    if j==0 or j==n-1 or i==j or i+j==n-1:
      print("*",end=" ")
    else:
      print(" ",end=" ")
  print()

  # for printing x

  n=int(input("enter the size"))
for i in range(n):
  for j in range(n):
    if i==j or i+j==n-1:
      print("*",end=" ")
    else:
      print(" ",end=" ")
  print()

  # printing triangle
  n=int(input("enter the size"))
for i in range(n):
  for j in range(n):
    if j==0 or i==n-1 or i==j:
      print("*",end=" ")
    else:
      print(" ",end=" ")
  print()

  # reverse triangle

  n=int(input("enter the size"))
for i in range(n):
  for j in range(n):
    if j==0 or i==0 or i+j==n-1:
      print("*",end=" ")
    else:
      print(" ",end=" ")
  print()

  # reflected triangle

  n=int(input("enter the size"))
for i in range(n):
  for j in range(n):
    if i==n-1 or j==n-1 or i+j==n-1:
      print("*",end=" ")
    else:
      print(" ",end=" ")
  print()

  # to print +

  n=int(input("enter the size"))
for i in range(n):
  for j in range(n):
    if i==n//2 or j==n//2:
      print("*",end=" ")
    else:
      print(" ",end=" ")
  print()

  # full triangle pattern

  n=int(input("enter the size"))
for i in range(n):
  for j in range(i): # for single for loop=("*"*i)
      print("*",end=" ")
  print()

  # reverse full pattern

  n=int(input("enter the size"))
for i in range(n,0,-1):
  for j in range(n-i):
    print("",end=" ")
  for k in range(i):
    print("*",end=" ")
  print()

# rhombus

n=int(input("enter the size"))
for i in range(1,n+1):
  for j in range(n-i):
      print('  ',end=" ")
  for k in range(2*i-1):
    print("* ",end=" ")
  print()
for i in range(n-1,0,-1):
  for j in range(n-i):
      print('  ',end=" ")
  for k in range(2*i-1):
    print("* ",end=" ")
  print()

# number pattern printing

n=int(input("enter the size"))
r=int(input("enter the size"))
for i in range(r):
  for j in range(i):
    print(n,end=" ")
    n+=1
  print()

# spiral 

n=int(input("enter the size"))
matrix=[[0]*n for _ in range(n)]
top,left=0,0
right,bottom=n-1,n-1
num=1
while top<=bottom and left<=right:
  for i in range(left,right+1):
    matrix[top][i]=num
    num+=1
  top+=1
  for i in range(top,bottom+1):
    matrix[i][right]=num
    num+=1
  right-=1
  for i in range(right,left-1,-1):
    matrix[bottom][i]=num
    num+=1
  bottom-=1
  for i in range(bottom,top-1,-1):
    matrix[i][left]=num
    num+=1
  left+=1
for row in matrix:
  for val in row:
    print(f"{val:3}",end='')
  print()

# traversal of matrix

matrix=[[1,2,3,4],[5,6,7,8],[9,10,11,12],[13,14,15,16]]
rows= len(matrix)
cols= len(matrix[0])
top,left=0,0
right,bottom=cols-1,rows-1
while top<=bottom and left<=right:
  for i in range(left,right+1):
    print(matrix[top][i],end=' ')
  top+=1
  for i in range(top,bottom+1):
    print(matrix[i][right],end=' ')
  right-=1
  for i in range(right,left-1,-1):
    print(matrix[bottom][i],end=' ')
  bottom-=1
  for i in range(bottom,top-1,-1):
    print(matrix[i][left],end=' ')
  left+=1

# alphabet spiral

n=int(input("enter the size"))
matrix=[[' ']*n for _ in range(n)]
ch=65
top,left=0,0
right,bottom=n-1,n-1
while top<=bottom and left<=right:
  for i in range(left,right+1):
    matrix[top][i]=chr(ch)
    ch+=1
    if ch>90:
      ch=65
  top+=1
  for i in range(top,bottom+1):
    matrix[i][right]=chr(ch)
    ch+=1
    if ch>90:
      ch=65
  right-=1
  for i in range(right,left-1,-1):
    matrix[bottom][i]=chr(ch)
    ch+=1
    if ch>90:
      ch=65
  bottom-=1
  for i in range(bottom,top-1,-1):
    matrix[i][left]=chr(ch)
    ch+=1
    if ch>90:
      ch=65
  left+=1
for row in matrix:
  for val in row:
    print(f"{val:3}",end='')
  print()

# user defined functions

*****(we have to take function name which is not a pre defined function
if we def starting it doesnot start reading from starting it will read from ending)*****

def hi():
  print("hello students") # call it as-->response of callee
  print("teju"*5) #prints the name 5 times
hi() #caller

# functions with parameters

def add(a,b):
  return a+b   ****# here we use a,b instead of student1,2 i.e, a,b are in 'add' statement in the line 4 near total we have used add so the a,b are stored in 'add' & to total****
student1=int(input("enter the money:"))
student2=int(input("enter the money:"))
total=add(student1,student2)
print("total amount:",total)

# functions with parameters/return value

def add(a,b): #can use(a,b)-->student1,student2
  print("total:",a+b) #can use(a+b)-->student1+student2
student1=int(input("enter the money:"))
student2=int(input("enter the money:"))
add(student1,student2)

# to find the value present in the function

def value():
  return 3.14159
result=value()
print("value in the function is",result)

# to find the value present in the function 'user defined'
def value():
  a=input()
  return a # if we want to add number we can add after 'a'-->(a+b)
result=value()
print("value in the function is",result)

# to lines printing at a time
def hi(name='guest'):
  print("hello",name)
a=input("enter data:")
hi()
hi(a) # here data is stored in-->def hi(name)

# pgrm
def info(name='unknown', age=0):
  print("NAME:",name)
  print("AGE:",age)
info("devi",21)
info("dev")
info(age=21)
info()
# all data types at a time
def cal(a,b):
  return a+b,a-b,a*b,a/b
a=int(input("enter a:"))
b=int(input("enter b:"))
sum,diff,pro,div=cal(a,b)
print("sum=",sum)
print("difference=",diff)
print("product=",pro)
print("divide=",div)

# printing minimum and maximum values
def num(a,b,c):
  return min(a,b,c),max(a,b,c)
a=int(input())
b=int(input())
c=int(input())
mini,maxi=num(a,b,c)
print("minimum=",mini)
print("maximum=",maxi)

# # write a function to count the lists of even  and odd numbers..calculate the even odd confirmantion in the function such that evaluated numbers list will be passed to the main program
def eo(numbers):
  e=0
  o=0
  for n in numbers:
    if n%2==0:
      e+=1
    else:
      o+=1
  return e,o
num=input("enter the numbers as space seperated:") 
num_list=list(map(int,num.split()))  ******# spliting the input string numbers into list*****
e,o=eo(num_list)
print("even count:",e)
print("odd count:",o) 

# lambda udv:arthematic op
# *******op= lambda a,b,c:(a+b)-c********
expo=lambda a:a**a
print(expo(3))

# 2 samples adding
add=lambda a,b:a+b
print(add(7,8))

# even odd boolean
is_even=lambda n:n%2==0
print(is_even(6))

# printing squares of some numbers
nums=[1,2,3,4,5,6,7,89,10]
sq=list(map(lambda n:n*n,nums))
print(sq)

# function within function/nested function
def outer():
  print("outer function")
  def inner():
    print("inner function")
  inner()
outer()

# function within functions
def cal(a,b):
  def add():
    return a+b
  def sub():
      return a-b
  def mul():
        return a*b
  print("addition",add())
  print("subtraction",sub())
  print("mutlipilaction",mul())
a=int(input("enter a num"))
b=int(input("enter b num"))
cal(a,b)

# pgrm
def mul_by(n):
  def inner(x): # call inner fun x=5
    return x*n #x*2 x*3
  return inner
times_2=mul_by(2) #n=2
times_3=mul_by(3) #n=3
print(times_2(5))
print(times_3(5))

# pgrm
def greet(text):
  def inner(name):
    return f"{text} {name}"
  return inner
hi=greet("hello")
print(hi("teju"))

# pgrm
def titled(title):
  def greet(name):
    return f"hello,{title}{name}"
  return greet
mr_greet=titled("mr.")
dr_greet=titled("dr.")
print(mr_greet("mine"))
print(dr_greet("teju"))

# pgrm
x=100
y=10
def display():
  x=22
  print("x= ",x)
  print("locally",x+y)
display()
print("x=",x)  
y=10
y=25
print(y)
print("globally",x+y)

# factorial-->(fact of 3=3*2*1=6)
fact=1
def factorial(n):
  global fact #---->we use global to call the variable outside the function --> fact is outside by using global we called it into pgrm/function
  fact=1
  for i in range(1,n+1):
    fact*=i
  return fact
num=int(input("enter number:"))
if num<0:
  print("no factorial for negative number")
else:
  factorial(num)
  print(f"factorial of {num} is",fact)

# recurssion
def factorial(n):
  if n==0 or n==1: #----->4 not equal to 0 & 1 then the if condition will be skipped
    return 1       #----->if num is 0 or 1 then it will return as 1
  return n*factorial(n-1)  # 4*3-->n-1=4-1------>4*3*2*1=24
num=int(input("enter the number")) #if num =4
value=factorial(num)
print(value)
