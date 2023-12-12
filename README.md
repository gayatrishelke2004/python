LIST
mylist=['phy','chem',2,5,8]
yourlist=[1,3,6,7,9,7]
print("mylist",mylist)
print("yourlist",yourlist)
mylist.append(4)
print(mylist)
yourlist.insert(2,10)
print(yourlist)
yourlist.sort()
print("sorted list in asc",yourlist)
yourlist.sort(reverse=True)
print("sorted list in des",yourlist)
mylist.pop(2)
print("mylist after pop of 2",mylist)
ourlist=mylist+yourlist
print("list after merging",ourlist)
total=sum(yourlist)
print("sum of mylist is",total)
maximum=max(yourlist)
print("max from list",maximum)
manimum=min(yourlist)
print("min from list",manimum)
cou=mylist.count(5)
print(cou)



TUPLES
mytup=(10,20,30)
print("mytuple",mytup)
yourtup=("pune","mumbai","delhi")
print("yourtuple",yourtup)
x=mytup.count(10)
print(x)
y=mytup.index(10)
print(y)
z=min(mytup)
print(z)
ourtup=mytup+yourtup
print("Add of tuples is",ourtup)
mylist=list(mytup)
print(mylist)
mylist.sort(reverse=True)
print(mylist)
you=mytup.count(10)
print(you)
a,b,c=yourtup
print("district",a)
print("state",b)
print("national",c)




DICT

mywallet={'diary':1,'ccards':2,'ddcards':2,'vcards':5}
print(mywallet)
mywallet['photo']=4
print(mywallet)
key="photo"
if key in mywallet.keys():
    print("true")
else:
    print("false")
mywallet.pop("photo")
print(mywallet)
mytup=tuple(mywallet)
print(mytup)
mylist=list(mywallet)
print(mylist)
sort=sorted(mywallet.items())
print(sort)
mywallet.copy()
print(mywallet)
mywallet.keys()
print (mywallet)
mywallet.items()
print (mywallet)
mywallet.values()
print(mywallet)
mywallet.clear()
print(mywallet)



SETS

eng={"jenny","serry","marry"}
man={"jenny",3,7,8,9}
print(eng)
print(man)
intersection=man&eng
print(intersection)
print(eng)
union=eng|man
print(union)
diff=man-eng
print(diff)
eng.discard("jenny")
print(eng)
sub=eng<=man
sup=man>=eng
print(sub)
print(sup)
myman=tuple(man)
print(myman)
myeng=list(eng)
print(myeng)
man.add("veery")
print(man)



PRIME NO

n=int(input("enter no"))
if n>1:
    for i in range(2,n):
        if(n%i)==0:
          print("is not prime",n)
        break
    else:
        print("is prime",n)
else:
       print("is not prime",n)



BEN TO DEC

num = input("Enter a binary number: ")
num = str(num)

# convert to decimal
dec = int(num, 2)
print("The decimal value of " + str(num) + " is " + str(dec))




DEC TO BIN

def dectobin(n):
    if n == 0:
        return 0
    else:
        return n % 2 + 10 * dectobin(n // 2)
  
n = int(input("Enter a decimal number: "))
print(dectobin(n)) 



FACTORIAL

num = int(input("Enter a number: "))

factorial = 1

# check if the number is negative, positive or zero
if num < 0:
   print("Sorry, factorial does not exist for negative numbers")
elif num == 0:
   print("The factorial of 0 is 1")
else:
   for i in range(1,num + 1):
       factorial = factorial*i
   print("The factorial of",num,"is",factorial)


FIBO SERIES

def Fib(n):
   if n <= 1:
       return n
   else:
       return (Fib(n - 1) + Fib(n - 2))  


n = int(input("Enter the Value of n: ")) 
print("Fibonacci series :")
for i in range(n):
   print(Fib(i),end = " ")


TABLE

n=int(input("Enter the number to print the tables for:"))
for i in range(1,11):
    print(n,"x",i,"=",n*i)


LARGEST NO

num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))
num3 = float(input("Enter third number: "))

if (num1 >= num2) and (num1 >= num3):
   largest = num1
elif (num2 >= num1) and (num2 >= num3):
   largest = num2
else:
   largest = num3

print("The largest number is", largest)




PYRAMID

n = int(input("enter no of rows))
for i in range(1, n+1):
    for j in range(n - i):
        print(' ', end='')
    for k in range(2 * i - 1):
        print('*', end='')
    print()


PALIDROME

string=input(("Enter a letter:"))  
if(string==string[::-1]):  
      print("The letter is a palindrome")  
else:  
      print("The letter is not a palindrome")  

REVERSE STRING

string=input(("Enter a letter:"))  
print(string[::-1]) 


ASCII VALUE

c = input(("enter the character"))
print("The ASCII value of '" + c + "' is", ord(c))


COUNT VOWELS

string=input("Enter string:")
vowels=0
for i in string:
      if(i=='a' or i=='e' or i=='i' or i=='o' or i=='u' or i=='A' or i=='E' or i=='I' or i=='O' or i=='U'):
            vowels=vowels+1
print("Number of vowels are:")
print(vowels)



PRINT VOWELS

text = input('Enter text: ')

for char in text:
    if char.lower() in 'aeiou':
        print(char)   

SWAP NO

x = 5
y = 10

x, y = y, x
print("x =", x)
print("y =", y)


CONCATENATE STRINGS

str1 = input("Enter the value of Str1: ")   
str2 = input("Enter the value of Str2: ")      
print("{} {}".format(str1, str2))     
str3 = "{} {}".format(str1, str2)     
print(str3)    



DATE AND TIME

from datetime import datetime
now = datetime.now()
print("now =", now)
dt_string = now.strftime("%d/%m/%Y %H:%M:%S")
print("date and time =", dt_string)



COMPOUND INTEREST


p = float(input("Enter the principle amount : "))
r = float(input("Enter the rate of interest : "))
t = float(input("Enter the time in the years: "))
ci =  p * (pow((1 + r / 100), t)) 
print("compound Interest : ", ci)


LEAP YEAR

year = int(input("enter year"))

if (year%400 == 0) or (year%4==0 and year%100!=0):
    print("Leap Year")
else:
    print("Not a Leap Year")

# python
