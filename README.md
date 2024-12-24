#Dictionary
#Examples
dictionary = {"Name":"Nivesh","Address":"Bokaro","Age":"23"}
print(dictionary["Age"])

#Iteration in Dictionary
for i in dictionary:
    print(i)
#Iteration in Dictionary @Using Value Functions.
for j in dictionary.values():
    print(j)
#Iteration in Dictionary @items Functions.
for m,n in dictionary.items():
    print(m,":",n)

#Dictionary top 5 functions.
#Examples
dictionary = {"Name":"Nivesh","Address":"Bokaro","Age":"23"}

print(dictionary.get("Name"))    #using get
print(dictionary.items())        #using items
print(dictionary.keys())          #using keys
print(dictionary.values())        #using value
print(dictionary.copy())          #using copy 

#write a python program to sort a dictionary by vale.
data = {"a":1,"b":6,"c":3,"d":100,"e":17}
print(sorted(data.values()))

#write a python script to print a dictionary where the keys are numbers between 1 and 15 and tha value are square of keys.
datas = {}
for j in range (1,16):
       print(j*j)

#write a program to multiply all the items in a dictionary.
nivesh = {"a":2,"b":4,"c":16}
product=1
for i in nivesh.values():
       product *= i
       print(product)

#write a python program to sort a dictionary by key.
key = {96:"a",177:"z",50:"b",12:"d"}
print(sorted(key.keys()))


#write a program to find max and min in a set.
name = (1,1,2,3,64,57,3,7)
print(max(name))
print(min(name))

#write a program to find common elements in three list sets.
a = {1,2,3,4,5}
b = {9,8,7,6,5}
c = {2,4,6,8,5}
print(a.intersection(b).intersection(c))

#write a program to find difference between two sets.
x = {1,2,3,4,5}
z = {9,8,7,6,5}
print(x.difference(z))

#write a python program to remove an items from a set if is present in the set.
k = {2,4,56,93,0,3}
print(k)
while k:
    p = input("if you want to remove any number please type / exit : ")
    if p.lower() == "exit":
            break
else:
    if p.isdigit():
        p = int(p)
        if p == k:
            k.remove(p)
            print("Your given number",p,"is remove")
        else:
            print("The given is not present in data")
    else:
        print("The given you have mention is not a Numrical")
print(k)

#wtite a program to check if a set is a subset of another set.
w = {1.2,3,4,5}
y = {2,3,4}
print(y.issubset(w))

#funcrions paramenter and arguments 1
def nivesh(x,y):
    print(x+y)
nivesh(98,56)

#funcrions paramenter and arguments2
def nivesh(*name):
    print("hello, my name is ",name[1])
nivesh("nivesh","kumar","singh")

#return statements and Recursion in python
def nivesh():
    return("only this value is return")            #functions
print(nivesh())

#Recursion in python 1
#In revesion time create and program to take the user intput and factorise 
def fact(n):
    if n == 1:
        return 1
    else:
        return n * fact(n-1)
print(fact(5))

#Recursion in python 2
def factorial(n):
    if n < 0:
        raise ValueError("Factorial is not defined for negative numbers.")
    elif n == 0:
        return 1
    else:
        return n * factorial(n  - 1)

user_input = int(input("Give the number to factorize: "))
result = factorial(user_input)
print("The factorial of {user_input} is {result}")

#lambda
a = lambda b : b*5
print(a(4))

x = 10 # global variable
def my_function():
                #  if you want to change the global x value the use (global x ↵ x = 9)
    y = 5 # local variable
    print(y)   
my_function()
print(x)
print(y) # this will cause an error because y is a local variable
# and is not accessible outside of the function

# write a function to find maximum of three numbers in python.
a = int(input("1st :- "))
b = int(input("2nd :- "))
c = int(input("3rd :- "))

def nivesh (a,b,c):
    if a >= b and a >= c:
        return a
    elif b >= a and b >= c:
        return b
    else:
        return c
print(nivesh(a,b,c))

#write a python function to create and a list where the value are square of number between 1 and 30.
def square ():
    return[i*i for i in range(1,31)]

print(square())

#Write a python function that taken a number as a parameter and check if the number is prime or not.g n  knjkl
def is_prime(num):
    if num < 2:
        return False
    for i in range(2, int(num ** 0.5) + 1):
        if num % i == 0:
            return False
    return True

prime_numbers = [num for num in range(1, 31) if is_prime(num)]
print("Prime numbers between 1 and 30:", prime_numbers)

# 2 method
def add(numbers):
    if len(numbers) == 1:  # Base case for recursion
        return numbers[0]  # If the list has only one number, return that number.
    else:  # Recursive case
        return numbers[0] + add(numbers[1:])  
        # Add the first number in the list to the result of the function
        # called with the rest of the list (excluding the first number).

print(add([12, 4, 5, 6, 7, 8]))
# Call the function with a list of numbers and print the result.

#write a python program to solve the fibonacci sequences using Recursion.
def fibo(num):
    if num == 1:
        return 0  # The first Fibonacci number is 0
    elif num == 2:
        return 1  # The second Fibonacci number is 1
    else:
        # Recursive case: The Fibonacci number is the sum of the previous two
        return fibo(num - 1) + fibo(num - 2)

# Get the 7th Fibonacci number
print(fibo(7))

import datetime
print(datetime.datetime.now())     #module datetime


# module
#datetime

import datetime
print(datetime.datetime.now())
x=datetime.datetime(2002,10,27)
print(x.strftime("%A")) # try (a-z) or (A-Z).

#random
import random
print(random.randint(7,70))
z=["HEAD","TAILS"]
print(random.choice(z))

#math
import math
print(max(1,78,56))
print(pow(4,9))
print(math.sqrt(89754675)) #.
print(abs(-78))
print(math.floor(78.3)) #.
print(math.ceil(78.5)) #.

#create module also watch #youtube Automate with Rakesh ((((((((Alias)))))))
import noted as m2 #m2=Alias
m2.greeting ("nivesh")
![image](https://github.com/user-attachments/assets/705ddc92-2133-48f8-92c3-bff008ff8521)

import numpy
d=numpy.array([10,20,89,90])
print(d[0:2])

import numpy as ni
d=ni.array([[10,20,89,90],[50,81,91,78]])
print(d[1:3,1:3])

import numpy as ni
d=ni.array([[10,20,89,90],[50,81,91,78]])
print([d[1,1:3],d[0,1:3]])

import numpy as ni
d=ni.array([[10,20,89,90],[50,81,91,78]])
print([d[1,1:3],d[0,1:3]])
print(ni.shape(d))      # shape
print(ni.size(d))       #size
print(ni.ndim(d))       #number dimension
print(d.dtype)      #how many bit will store your data

import numpy as nv
a = [[56,89,78,56],[45,58,56,78]]
arr = nv.array(a)
print(nv.array(a))
print(arr.shape)
print(len(a))
print(arr.ndim)
print(arr.size)
print(arr.dtype)
print(type(arr))
print(arr.astype(float))

import numpy as nv
a = [[56,89,78,56],[45,58,56,78]]
arr = nv.array(a)
print(nv.array(a))
print(arr.shape)   #row and columns
print(len(a))      #output 2 because [ ] ,[ ] nested
print(arr.ndim)    #number dimension
print(arr.size)    # output 8 elements
print(arr.dtype)    # data types
print(type(arr))     # types of variable
print(arr.astype(float))    #types convert

#mathmatics operation and funtions on arrays.

import numpy as np
# Correctly define 2D arrays
arr1 = np.array([[20, 40], [50, 60]])
arr2 = np.array([[50, 60], [70, 80]])
arr3 = np.array([5])
# Perform mathematical operations
print("Addition:\n", np.add(arr1, arr2))       # Element-wise addition
print("Subtraction:\n", np.subtract(arr1, arr2))  # Element-wise subtraction
print("Division:\n", np.divide(arr1, arr2))   # Element-wise division
print("power:\n", np.power(arr1,arr3))        # ELements-wise power

# concatenate
import numpy as np
arr1 = np.array([[30, 40],[50,80]])
arr2 = np.array([[5, 5],[40,60]])
print(np.concatenate([arr1, arr2]))
print(np.concatenate([arr1,arr2],axis=1))
print(np.concatenate([arr1,arr2],axis=0))
print(np.hstack([arr1,arr2]))       #horizonatal Concatenate
print(np.vstack([arr1,arr2]))       #vertical concatenate

a =np.array([56,58,96,87,74])
print(np.array_split(a,3))        #you can also use 2d data

import numpy as ni
a=ni.array([50,12,56,75,25])
print(a)
print(ni.append(a,56))
h = ([56,89,73])
print(ni.append(a,h))
print(a)
print(ni.insert(a,3,56))
print(ni.delete(a,2))
s = ni.detete(a,5)
print(a)                #every time you just add and delete something in the array the will be not futher changes in the array you have to create like that s = ni.detete(a,5)

import numpy as xp
a = xp.array([56,85,89,57,44])
print(xp.sort(a))
print(xp.where(a == 44))
print(xp.where(a % 2 == 0))
print(xp.searchsorted(a,1))

import numpy as xp
a = xp.array([35,85,89,57,90])
print(xp.sort(a))
print(xp.where(a == 44))
print(xp.where(a % 2 == 0))
print(xp.searchsorted(a,1))
print(a>40)
print(a[a>40])
print(a[a%2==0])
print(a[a%2==1])

import numpy as xp
a = xp.array([35,85,89,57,90])
print(xp.sum(a))
print(xp.max(a))
print(xp.min(a))
print(xp.size(a))
print(xp.mean(a))
print(xp.median(a))
print(xp.cumsum(a))

import numpy as xp
p = xp.array([35,85,89,57,90])
q = xp.array([5,6,8,9,2])

c= xp.cumprod([p,q],axis=0)
print(c)
print(c[1].sum())

import numpy as xp
import statistics as pp
p = xp.array([35,85,89,57,90])
print(pp.mode(p))
print(xp.std(p))
print(xp.var))         #variantions double od standard deviation

import numpy as np
import statistics as st
price = [700,600,500,400,300]
sales = [80,60,50,40,20]
print(np.corrcoef([price,sales]))        1 is directly proportion / -1 is inversaly proportion / 0 no relation

Pandas
import pandas as pd
data={"Name":["Nivesh","kumar","style"],
    "Age":[20,21,22],
    "Salary":[4000,5000,6000]}
print(pd.DataFrame(data))

import pandas as pd
data = pd.read_csv("C:/Users/nives/OneDrive/Desktop/New folder/Book.csv", encoding='utf-8')
print(data)

import pandas as pd
data = pd.read_excel("C:/Users/nives/OneDrive/Desktop/New folder/Book.xlsx")
print(data)

import pandas as pd
data = pd.read_excel("C:/Users/nives/OneDrive/Desktop/New folder/Book.xlsx")
print(data.info())

import pandas as pd
data = pd.read_excel("C:/Users/nives/OneDrive/Desktop/New folder/Book.xlsx")
print(data.describe())

import pandas as pd
data = pd.read_excel("C:/Users/nives/OneDrive/Desktop/New folder/Book.xlsx")
print(data.isnull())

import pandas as pd
data = pd.read_excel("C:/Users/nives/OneDrive/Desktop/New folder/Book.xlsx")
print(data.isnull().sum())

import pandas as pd  # Use pandas for Excel file handling

# File path
filetype = "C:/Users/nives/OneDrive/Desktop/python data analytics file/Book.xlsx"

# Read the Excel file
data = pd.read_excel(filetype)
print("Mean Salary:", data["Salary"].mean())


import pandas as pd

# Correct the file path (assuming the path is case-sensitive)
file_path = "C:/Users/nives/OneDrive/Desktop/New folder/Book.xlsx"

# Correct the file path (assuming the path is case-sensitive)
file_path = "C:/Users/nives/OneDrive/Desktop/New folder/Book.xlsx"

# Read the Excel file
data = pd.read_excel(file_path)

# Remove duplicate rows
data = data.drop_duplicates()            #use this on varriable or print

data ["Job Title"] = data ["Job Title"].fillna("Clerk")        #fillna = fill NaN means blanck fill with data.
print(data)


import pandas as pd
filetype =pd.read_excel("C:/Users/nives/OneDrive/Desktop/python data analytics file/ESD.xlsx")
print (filetype)
filetype.loc[filetype["Bonus %"] == 0, "GetBonus %"] = "No Bonus"
filetype.loc[filetype["Bonus %"] > 0, "GetBonus %"] = "Bonus"            #create a new columns & also if use.
print(filetype)
print(filetype.head(10))

import pandas as pd
data = pd.read_excel("practice_1.xlsx")                #use in jupyter note book & the file practice_1 is avilable on local file where jupyter is connceted
print(data)
data["Full Name"]=data["Name"].str.capitalize() + " " + data["Sername"].str.capitalize()
print(data)

import pandas as pd
#dictonary
data = {
    "Months":[
        "January","February","March","April","May",
        "June","July","August","September","October",
        "November","December"
    ]
}
#Dataframe
a = pd.DataFrame(data)
print(a)
#function
def extract(value):
    return value[0:3]
a["Short Months"] = a["Months"].map(extract)            #data trim like january = jan
print(a)

gb=dbz.groupby("Department").agg({"Gender":"count"})
print(gb)                                                #for counting gender in each department

gb=dbz.groupby(["Department","Gender"]).agg({"EEID":"count"})
print(gb)                                                #For counting gender in each department with gender male and female base

import pandas as pd
dbz=pd.read_excel("ESD.xlsx")
data=dbz.groupby(["Country"]).agg({"Age":"mean"})         #mean,avg,max,
print(data)

import pandas as pd
data1 = {"Emp ID":["E1","E2","E3","E4","E5",],
         "Name":["Nivesh","Kumar","Singh","Nikita","Ram"],
         "Age":[20,22,24,18,17]}
data2 = {"Emp ID":["E1","E2","E3","E6","E8",],
         "Salary":[20000,25000,16000,18000,12000]}
df1 = pd.DataFrame(data1)
df2 = pd.DataFrame(data2)
print(df1)
print()        #print() mean nothing but blank
print(df2)
print(pd.merge(left=df1, right=df2, on = "Emp ID", how = "left"))            #if main table is left table
print(pd.merge(left=df1, right=df2, on = "Emp ID", how = "right"))           #if main table is right table


#if you want to merge two seprate table with equal columns tittle that called CONCATENATE 
import pandas as pd
data1 = {"Emp ID":["E1","E2","E3","E4","E5",],
         "Name":["Nivesh","Kumar","Singh","Nikita","Ram"],
         "Age":[20,22,24,18,17]}
data2 = {"Emp ID":["E6","E7","E8","E9","E10",],
         "Name":["Nikita","Kumari","Dhangi","Ram","Nath"],
         "Age":[22,26,25,20,22]}
df1 = pd.DataFrame(data1)
df2 = pd.DataFrame(data2)

print(pd.concat([df1,df2]))                #CONCATENATE two table merge

#updata Data
import pandas as pd
data1 = {"Emp ID":["E1","E2","E3","E4","E5",],
         "Name":["Nivesh","Kumar","Singh","Nikita","Ram"],
         "Age":[20,22,24,18,17]}
data2 = {"Emp ID":["E1","E2","E3","E4","E5",],
         "Salary":[20000,25000,16000,18000,12000]}
df1 = pd.DataFrame(data1)
df2 = pd.DataFrame(data2)
df3 = df2.copy()
df3.loc[0,"Salary"]=25000
df3.loc[1,"Salary"]=50000
df3.loc[2,"Salary"]=25000
df3.loc[3,"Salary"]=16000
df3.loc[4,"Salary"]=25000
print(pd.merge(df1,df2))
print()
print(pd.merge(df1,df3))
print(df2.compare(df3))         #compare one data tabel to Another Data table
print(df2.compare(df3,align_axis =0))
print(df2.compare(df3,keep_equal= True))
print(df2.compare(df3,keep_equal= False))
print(df2.compare(df3,keep_shape= True))

import pandas as pd
dic = {
    "keys":["k1","k2","k1","k2"],
    "name":["Nivesh","Kumar","Singh","Dhangi"],
    "house":["red","blue","green","pink"]}
df = pd.DataFrame(dic)
print(df)
print()
print(df.pivot(index="keys", columns="name", values="house"))                    #pivot with index and columns & values

import pandas as pd
df = pd.DataFrame({
    'Name': ['Alice', 'Bob', 'Charlie', 'David', 'Eve'],
    'Math': [90, 85, 78, 92, 88],
    'Physics': [88, 92, 84, 91, 89],
    'Chemistry': [78, 89, 80, 87, 82],
    'Biology': [95, 93, 88, 94, 90],
    'History': [87, 91, 75, 89, 86]
})
print(df)
melt_df = pd.melt(df,id_vars="Name")         #if you want to change new columns name variable us this code in this code  like i take subject Var_name="Subject" / do you want to change value use vlaue_name="book"
melt_df                # jupyter note you need to print last print(melt_df) you ccan use Melt

import matplotlib.pyplot as plt
y = [40, 80, 90, 2, 15]
x = ["A", "B", "C", "D", "E"]
#colour=["red","pink","green","yellow","white"]
plt.bar(x, y,color="red")                #if you want to how many things that wiil use ...|) shift+tab a pop-pop show search all
plt.xlabel("some",fontsize=17)
plt.ylabel("something")
plt.title("nivesh")
plt.show()

import matplotlib.pyplot as plt
import pandas as pd
data = pd.read_excel("C:/Users/nives/OneDrive/Desktop/python data analytics file/exp.xlsx")
df = pd.DataFrame(data)
plt.bar(df["Payment Mode"],df["Amount"])
plt.xlabel("some",fontsize=17)
plt.ylabel("something")
plt.title("nivesh")
plt.show()

import matplotlib.pyplot as plt
import pandas as pd
data = pd.read_excel("C:/Users/nives/OneDrive/Desktop/python data analytics file/exp.xlsx")
df = pd.DataFrame(data)
grouped_by = df.groupby("Payment Mode")["Amount"].sum()
print(grouped_by)
plt.bar(grouped_by.index,grouped_by.values)
plt.show()

import pandas as pd
import matplotlib.pyplot as plt
x = ["A","B","C","D"]
y = [10,50,25,40]
z = [90,70,52,25]
plt.plot(x,y,marker="^",linestyle="--")        #if you want to add some new style find SHIFT+TAB
plt.plot(x,z,color="pink")
plt.show()

import matplotlib.pyplot as plt
import numpy as np
x = np.random.randint(1,20,50)
y = np.random.randint(10,100,50)
plt.scatter(x,y,marker = "^",color = "red")
plt.show()

import matplotlib.pyplot as plt
import numpy as np
x = np.random.randint(1,20,50)
y = np.random.randint(10,100,50)
colour=np.random.randint(10,100,50)
plt.scatter(x,y,marker = "^",c=colour,cmap="viridis",)        #cmap="hot"
plt.colorbar()
plt.show()

import matplotlib.pyplot as plt
brands = ["Xiaomi", "Vivo", "Samsung", "Realme", "OPPO", "OnePlus", "Apple"]
share = [20.67,18.22,13.69,13.45,11.71,4.82,4.10]
colour = ["red","blue","pink","black","green","orange","brown"]
ex = [0,0,1,0,0,0,0]
plt.pie(share, labels=brands, colors=colour, explode = ex, shadow=True,autopct ="%f",startangle=90)
plt.title("Mobile Market Share of India")                    #pie chart
plt.show()



