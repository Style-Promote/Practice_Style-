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
    return("only this value is return")
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


