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

