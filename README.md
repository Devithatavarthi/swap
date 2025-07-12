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

# subset check
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

#  set with lists
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

# code for if condition to check,whether the person is eligible to vote or not 
#age>18
age=int(input("enter the age of the person:"))
if age>=18:
    print("eligible to vote")
#  code for determinig the character entered by user 
    char=input("press any key:")
if char.isalpha():
    print(char,"is a character")
    if char.isdigit():
        print(char,"is a digit")
    if char.isspace():
        print(char,"is a space")
#  code to check the number is positive or not
num=int(input("enter a number:"))
if num>0:
    print(num,"is a positive")
    if num<0:
        print(num,"is negitive")
        if num==0:
            print(num,"is zero")
#  program to enter any char if the enterd char is in  and vice versalowercase than covert the char into uppercase and viceversa '''
ch=input("enter a char from a to z")
if ch>='A' and ch<='Z':
    ch=ch.lower()
    print("the entered character was in uppercase...lower:"+ch)
else:
    ch=ch.upper()
    print("the entered character was in lowercase...upper:"+ch)
#  code for checking the interval of a given number
num=int(input("enter the number:"))
if num>=0 and num<=10:
    print(num,"is in 0-10 range")
elif num>=11 and num<=20:
    print(num,"is in 11-20 range")
elif num>=21 and num<=30:
    print(num,"is in 21-30 range")
else:
    print("out of range")
  #  if -else statement
num=int (input("enter the number:"))
if num%2==0:
    print(num,"is even")
else:
    print(num,"is odd")      
   #  if elif else startment 
a=int(input("enter a:"))
b=int(input("enter b:"))
if a>b:
    print("largest :",a)
elif a<b:
    print("largest :",b)
else:
    print("both numbers are equal") 
# nested if
    num=int(input("enterr the number"))
if num>0:
    print("positive")
    if num%2==0:
        print("even")
    else:
        print("odd")
else:
    print("numbrt isnon positive")          
  # loop
num= int(input("enter a number :"))
loop=0
while loop<num:
    print("DEVI")
    loop+=1          
#  frist n natural number upto 50
num=int(input("enter anumber"))
while num>=1:
    print(num)
    num-=1
# amstrong number
num=int(input("enter the number: "))
temp=num
n=len(str(num))
sum=0
while temp>0:
    digit=temp%10
    sum +=digit**n
    temp//=10
print("latest value of sum:",sum)
print("latest value of temp:",temp)
if sum==num:
    print("amstrong number")
else:
    print("not amstrong number")
# nivens number
num=int(input("enter the number"))
temp=num
sum=0
while temp>0:
    digit=temp%10
    sum+=digit
    temp//=10
if num%sum==0:
    print(" niven's harshad number")
else:
    print("not nivens number")

# Program to print squares of numbers from 1 to 10

for number in range(1, 11):
    square = number ** 2
    print(f"The square of {number} is {square}")
   #  patterns
   n=int(input("enter the size"))
for i in range(n):
    for j in range(n):
        print('*',end='')
    print()
    
# patterns
 n=int(input("enter the size"))
for i in range(n):
  for j in range(n):
    if i==0 or i==n-1 or j==0 or j==n-1:
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
# triangle
  n=int(input("enter the size"))
for i in range(n):
  for j in range(n):
    if j==0 or i==n-1 or i==j :
      print("*",end=" ")
    else:
      print(" ",end=" ")
  print()
  # reverse triangle
  n=int(input("enter the size"))
for i in range(n):
  for j in range(n):
    if i==0 or j==n-1 or i==j :
      print("*",end=" ")
    else:
      print(" ",end=" ")
  print()
  # plus
  n=int(input("enter the size"))
for i in range(n):
  for j in range(n):
    if i==n//2 or j==n//2:
      print("*",end=" ")
    else:
      print(" ",end=" ")
  print()
  # pyramid
  n=int(input("enter the size"))
for i in range(n):
  for j in range(n-i):
      print("",end=" ")
  for k in range(i):
    print("*",end=" ")
  print()
  # reverse pyramid
  n=int(input("enter the size"))
for i in range(n,0,-1):
  for j in range(n-i):
      print('  ',end=" ")
  for k in range(2*i-1):
    print("* ",end=" ")
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
  # sperial
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
  # matrix
  matrix=[[1,2,3,4],[5,6,7,8],[9,10,11,12,],[13,14,15,16]]
row=len(matrix)
cols=len(matrix[0])
top,left=0,0
right,bottom=cols-1,row-1
while top<=bottom and left<=right:
  for i in range(left,right+1):
    print(matrix[top][i],end=' ')
  top+=1
  for i in range(top,bottom+1):
    print(matrix[right][i],end=' ')
  right-=1
  for i in range(right,left-1,-1):
    print(matrix[bottom][i],end=' ')
  bottom-=1
  for i in range(bottom,top-1,-1):
    print(matrix[left][i],end=' ')
  left+=1
  # travaesal 
n=int(input("enter the size:"))
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
      print(f"{val:3}",end=' ')
    print()
 # functions
def hi(): #callee
  print("hello students") # responses of callee
  print("devi "*5)
hi() # caller
# functions parameters with return values
def add(a,b):
  return a+b
student1=int(input("enter the money:"))
student2=int(input("enter the money:"))
total=add(student1,student2)
print("total amount:",1total)
# functions parameters/return values
def add(student1, student2):
  print("total:",student1+student2)
student1=int(input("enter the money:"))
student2=int(input("enter the money:"))
add(student1,student2)
# storeing data in value
def value():
  return 3.14159
result=value()
print("value on the function is",result)
# user defined
def get_name():
  name=input("enter the name: ")
  return name
username=get_name()
print("welcome",username)
# names storing data 
def hi(name):
  print("hello",name)
a=input("enter data:")
hi(a)
# artimatic 
def cal(a,b):
  return a+b,a-b,a*b,a/b
a=int(input("enter a:"))
b=int(input("enter b :"))
sum, diff, pro, div =cal(a,b)
print("sum=",sum)
print("subtract=",diff)
print("product",pro)
print("divide=",div)
# maximum and minimum
def max_min(a,b,c):
  return max(a,b,c),min(a,b,c)
a=int(input("enter a:"))
b=int(input("enter b:"))
c=int(input("enter c:"))
maxi,mini=max_min(a,b,c)
print("maximum:",maxi)
print("minimum:",mini)
# write a function to count the lists of even  and odd numbers..calculate the even odd confirmantion in the function such that evaluated numbers list will be passed to the main program
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
num_list=list(map(int,num.split()))
e,o=eo(num_list)
print("even count:",e)
print("odd count:",o)
# lambdan udv: arthmetic op
# op=lambda a,b,c:(a+b)-c
expo=lambda a:a**a
print(expo(3))
# sum
add=lambda a,b:a+b
print("sum:",add(7,8))
# lambda statement
is_even=lambda n: n%2==0
print("is 6 even",is_even(6))
# sq of numbers using lambda 
nums=[1,2,3,4,5,6,7,8,9,10]
sq=list(map(lambda n:n**2,nums))
print(sq)
# fwf
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
# mul fwf
def mul_by(n):
  def inner(x): # call inner function x=5
    return x*n #x*2    x*3  
  return inner
times_2=mul_by(2) #n=2,
times_3=mul_by(3) #n=3,
print(times_2(5))
print(times_3(10))
# inner calle
def greet(text):
  def inner(name):
    return f"{text},{name}!!!!!"
  return inner
hi=greet('helo')
print(hi('deva'))
# title calle
def titled(title):
  def greet(name):
    return f"{title}{name}"
  return greet  
mr_greet=titled("mr.")
dr_greet=titled("dr.")
print(mr_greet("deva"))
print(dr_greet("deva"))


